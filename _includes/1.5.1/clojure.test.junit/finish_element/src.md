## source
{% highlight clojure linenos %}
(defn finish-element
  [tag pretty]
  (set! *depth* (dec *depth*))
  (if pretty (indent))
  (print (str "</" tag ">"))
  (if pretty (println)))
{% endhighlight %}