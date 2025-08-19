# S-U-Sonbhadra-Express-
Your grocery needs, delivered! S U Sonbhadra Express offers fresh, high-quality groceries to your doorstep in Robertsganj. Our user-friendly website ensures a seamless shopping experience. We're dedicated to customer satisfaction and fast, reliable delivery. Shop with us for a convenient way to get what you need, when you need it.
Screen1.Initialize
    set LabelWelcome.Text to "Welcome to S U Sonbhadra Express"
    ProductsList.Elements = ["Rice - 50/kg", "Sugar - 45/kg", "Oil - 120/litre"]
    ListView1.AfterPicking
    set SelectedProduct = ListView1.Selection
    call Notifier1.ShowMessage("You selected " + SelectedProduct)
   ButtonSubmit.Click
    set OrderName = TextBoxName.Text
    set OrderAddress = TextBoxAddress.Text
    set OrderPhone = TextBoxPhone.Text
    set OrderProduct = TextBoxProduct.Text
    call Notifier1.ShowMessage("Order Placed Successfully! Thank you " + OrderName)
    ButtonCall.Click
    call ActivityStarter.StartActivity
