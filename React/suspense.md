### Dynamically load 
Sample code to implement Lazy loading component.

````js
import React, { Suspense } from "react";
import Loader from "./components/Loader";

const LazyComponent = React.lazy(() => import("./components/LazyComponent"));

function ParentComponent() {
  return (
    <div className="a-class-name">
        <Suspense fallback={<Loader label="Loading..."></Loader>}>
            <LazyComponent />
        </Suspense>
    </div>
  )
}

````
