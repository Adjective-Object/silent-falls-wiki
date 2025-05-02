- Welcome to the Silent Falls Wiki! To get started, check out the [[Silent Falls, USA]] page, or browse the query indices below:
- #+BEGIN_QUERY
  {:title "Sessions"
   :query [:find ?name
           :in $ ?tag
           :where
             [?t :block/name ?tag]
             [?p :block/tags ?t]
             [?p :block/name ?name]
         ]
   :inputs ["sessions"]
   :view (fn [result]
        [:ul
            (for [page result]
                [:li [:a {:href (str "#/page/" page)} page]]
             )
        ]
      )
   }
  #+END_QUERY
- #+BEGIN_QUERY
  {:title "Stories"
   :query [:find ?name
           :in $ ?tag
           :where
             [?t :block/name ?tag]
             [?p :block/tags ?t]
             [?p :block/name ?name]
         ]
   :inputs ["stories"]
   :view (fn [result]
        [:ul
            (for [page result]
                [:li [:a {:href (str "#/page/" page)} page]]
             )
        ]
      )
   }
  #+END_QUERY
- #+BEGIN_QUERY
  {:title "Characters"
   :query [:find ?name
           :in $ ?tag
           :where
             [?t :block/name ?tag]
             [?p :block/tags ?t]
             [?p :block/name ?name]
         ]
   :inputs ["characters"]
   :view (fn [result]
        [:ul
            (for [page result]
                [:li [:a {:href (str "#/page/" page)} page]]
             )
        ]
      )
   }
  #+END_QUERY
- #+BEGIN_QUERY
  {:title "Factions"
   :query [:find ?name
           :in $ ?tag
           :where
             [?t :block/name ?tag]
             [?p :block/tags ?t]
             [?p :block/name ?name]
         ]
   :inputs ["factions"]
   :view (fn [result]
        [:ul
            (for [page result]
                [:li [:a {:href (str "#/page/" page)} page]]
             )
        ]
      )
   }
  #+END_QUERY
- #+BEGIN_QUERY
  {:title "Locations"
   :query [:find ?name
           :in $ ?tag
           :where
             [?t :block/name ?tag]
             [?p :block/tags ?t]
             [?p :block/name ?name]
         ]
   :inputs ["locations"]
   :view (fn [result]
        [:ul
            (for [page result]
                [:li [:a {:href (str "#/page/" page)} page]]
             )
        ]
      )
   }
  #+END_QUERY