# django-simple-pagination
Django Simple Pagination Script 

# views.py
   faqs = Faq.objects.all()
   data = {}
   faqs, pagination_info = get_paginated_objects(faqs, page, 5)
    data.update(
        {
            'faqs': faqs,
            'pagination_info': pagination_info
        }
    )
    return data
    
  
