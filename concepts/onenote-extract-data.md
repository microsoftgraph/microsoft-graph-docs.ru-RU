# <a name="use-onenote-api-div-tags-to-extract-data-from-captures"></a><span data-ttu-id="e351e-101">Использование тегов div API OneNote для извлечения данных из записанного содержимого</span><span class="sxs-lookup"><span data-stu-id="e351e-101">Use OneNote API div tags to extract data from captures</span></span> 

<span data-ttu-id="e351e-102">*__Относится к:__ обычные записные книжки в OneDrive | корпоративные записные книжки в Office 365*</span><span class="sxs-lookup"><span data-stu-id="e351e-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>

<span data-ttu-id="e351e-103">Используйте API OneNote, чтоб извлекать данные визитных карточек с изображения или данные из рецептов и описаний товаров по URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="e351e-103">Use the OneNote API to extract business card data from an image, or recipe and product data from a URL.</span></span>

<a name="attributes"></a>
## <a name="extraction-attributes"></a><span data-ttu-id="e351e-104">Атрибуты извлечения</span><span class="sxs-lookup"><span data-stu-id="e351e-104">Extraction attributes</span></span>

<span data-ttu-id="e351e-105">Чтобы извлекать и преобразовывать данные, просто включите элемент div, указывающий исходный контент, метод извлечения и резервное действие в запрос [create-page](onenote-create-page.md) или [update-page](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="e351e-105">To extract and transform data, simply include a div that specifies the source content, extraction method, and fallback behavior in your [create-page](onenote-create-page.md) or [update-page](onenote_update_page.md) request.</span></span> <span data-ttu-id="e351e-106">API отображает извлеченные данные на странице в простом для чтения формате.</span><span class="sxs-lookup"><span data-stu-id="e351e-106">The API renders extracted data on the page in an easy-to-read format.</span></span> 

```
<div
  data-render-src="image-or-url"
  data-render-method="extraction-method"
  data-render-fallback="fallback-action">
</div>
```

<span data-ttu-id="e351e-107">**data-render-src**</span><span class="sxs-lookup"><span data-stu-id="e351e-107">**data-render-src**</span></span>

<span data-ttu-id="e351e-108">Источник контента.</span><span class="sxs-lookup"><span data-stu-id="e351e-108">The content source.</span></span> <span data-ttu-id="e351e-109">Это может быть изображение визитной карточки либо абсолютный URL-адрес страницы с рецептом или описанием товара.</span><span class="sxs-lookup"><span data-stu-id="e351e-109">This can be an image of a business card or an absolute URL from many popular recipe or product websites.</span></span> <span data-ttu-id="e351e-110">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e351e-110">Required.</span></span>

<span data-ttu-id="e351e-111">Для наилучших результатов используйте канонический URL-адрес, указанный в HTML-коде исходной веб-страницы (если он указан).</span><span class="sxs-lookup"><span data-stu-id="e351e-111">For best results when sending a URL, use the canonical URL defined in the  HTML of the source webpage, if one is defined. Example: <link rel="canonical" href="www.domainname.com/page/123/size12/type987" />.</span></span> <span data-ttu-id="e351e-112">Например, канонический URL-адрес может быть задан в исходной веб-странице следующим образом:</span><span class="sxs-lookup"><span data-stu-id="e351e-112">For example, a canonical URL might be defined in the source webpage like this:</span></span>

`<link rel="canonical" href="www.domainname.com/page/123/size12/type987" />` 


<span data-ttu-id="e351e-113">**data-render-method**</span><span class="sxs-lookup"><span data-stu-id="e351e-113">**data-render-method**</span></span>

<span data-ttu-id="e351e-114">Метод извлечения, который необходимо запустить.</span><span class="sxs-lookup"><span data-stu-id="e351e-114">The extraction method to run:</span></span> <span data-ttu-id="e351e-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e351e-115">Required.</span></span>

| <span data-ttu-id="e351e-116">Значение</span><span class="sxs-lookup"><span data-stu-id="e351e-116">Value</span></span> | <span data-ttu-id="e351e-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e351e-117">Description</span></span> |
|:------|:------|
| <span data-ttu-id="e351e-118">extract.businesscard</span><span class="sxs-lookup"><span data-stu-id="e351e-118">extract.businesscard</span></span> | <span data-ttu-id="e351e-119">Извлечение данных визитной карточки.</span><span class="sxs-lookup"><span data-stu-id="e351e-119">A business card extraction.</span></span> |
| <span data-ttu-id="e351e-120">extract.recipe</span><span class="sxs-lookup"><span data-stu-id="e351e-120">extract.recipe</span></span> | <span data-ttu-id="e351e-121">Извлечение рецепта.</span><span class="sxs-lookup"><span data-stu-id="e351e-121">A recipe extraction.</span></span> |
| <span data-ttu-id="e351e-122">extract.product</span><span class="sxs-lookup"><span data-stu-id="e351e-122">extract.product</span></span> | <span data-ttu-id="e351e-123">Извлечение описания товара.</span><span class="sxs-lookup"><span data-stu-id="e351e-123">A product listing extraction.</span></span> |
| <span data-ttu-id="e351e-124">extract</span><span class="sxs-lookup"><span data-stu-id="e351e-124">Extract</span></span> | <span data-ttu-id="e351e-125">Неизвестный тип извлечения.</span><span class="sxs-lookup"><span data-stu-id="e351e-125">An unknown extraction type.</span></span> |

<span data-ttu-id="e351e-126">Для наилучших результатов укажите тип контента (`extract.businesscard`, `extract.recipe` или `extract.product`), если вы его знаете.</span><span class="sxs-lookup"><span data-stu-id="e351e-126">For best results, specify the content type (`extract.businesscard`, `extract.recipe`, or `extract.product`) if you know it.</span></span> <span data-ttu-id="e351e-127">Если тип контента неизвестен, используйте метод `extract`, и API OneNote попытается автоматически определить тип.</span><span class="sxs-lookup"><span data-stu-id="e351e-127">For best results, specify the content type (business card, recipe, or product) if you know it. If  the type is unknown, you can use the extract method and the onnvshort API will try to auto-detect the type.</span></span>

<span data-ttu-id="e351e-128">**data-render-fallback**</span><span class="sxs-lookup"><span data-stu-id="e351e-128">**data-render-fallback**</span></span>

<span data-ttu-id="e351e-129">Резервное действие при неудачном извлечении.</span><span class="sxs-lookup"><span data-stu-id="e351e-129">The fallback behavior if the extraction fails:</span></span> <span data-ttu-id="e351e-130">Если атрибут не указан, по умолчанию используется значение **render**.</span><span class="sxs-lookup"><span data-stu-id="e351e-130">Defaults to **render** if omitted.</span></span> 

| <span data-ttu-id="e351e-131">Значение</span><span class="sxs-lookup"><span data-stu-id="e351e-131">Value</span></span> | <span data-ttu-id="e351e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e351e-132">Description</span></span> |
|:------|:------|
| <span data-ttu-id="e351e-133">render</span><span class="sxs-lookup"><span data-stu-id="e351e-133">render()</span></span> | <span data-ttu-id="e351e-134">Отображает исходное изображение или снимок веб-страницы с рецептом или товаром.</span><span class="sxs-lookup"><span data-stu-id="e351e-134">Renders the source image or a snapshot of the recipe or product webpage.</span></span> |
| <span data-ttu-id="e351e-135">Нет</span><span class="sxs-lookup"><span data-stu-id="e351e-135">none</span></span> | <span data-ttu-id="e351e-136">Не выполняет никаких действий.</span><span class="sxs-lookup"><span data-stu-id="e351e-136">Does nothing.</span></span><br /><span data-ttu-id="e351e-137">Этот параметр удобно использовать, если вы хотите всегда размещать снимок визитной карточки или веб-страницы на странице (в дополнение к извлеченному контенту).</span><span class="sxs-lookup"><span data-stu-id="e351e-137">Does nothing. This option is useful if you want to always include a snapshot of the business card or webpage on  the page in addition to any extracted content. Be sure to send a separate img element in the request.</span></span> <span data-ttu-id="e351e-138">Обязательно отправляйте отдельный элемент `img` в запросе, как показано в примерах.</span><span class="sxs-lookup"><span data-stu-id="e351e-138">Be sure to send a separate `img` element in the request, as shown in the examples.</span></span> |

<a name="biz-card"></a>
## <a name="business-card-extractions"></a><span data-ttu-id="e351e-139">Извлечение данных визитной карточки</span><span class="sxs-lookup"><span data-stu-id="e351e-139">Business card extractions</span></span>

<span data-ttu-id="e351e-140">API OneNote пытается найти и отобразить следующую контактную информацию на основе изображения визитной карточки человека или компании.</span><span class="sxs-lookup"><span data-stu-id="e351e-140">The onnvshort API tries to find and  render the following contact information  based on an image of a person's or company's business card.</span></span>


- <span data-ttu-id="e351e-141">Имя</span><span class="sxs-lookup"><span data-stu-id="e351e-141">Name</span></span>
- <span data-ttu-id="e351e-142">Название</span><span class="sxs-lookup"><span data-stu-id="e351e-142">Title</span></span>
- <span data-ttu-id="e351e-143">Организация</span><span class="sxs-lookup"><span data-stu-id="e351e-143">Organization</span></span>
- <span data-ttu-id="e351e-144">Номер телефона/факса</span><span class="sxs-lookup"><span data-stu-id="e351e-144">Phone and fax numbers</span></span>
- <span data-ttu-id="e351e-145">Почтовый и фактический адрес</span><span class="sxs-lookup"><span data-stu-id="e351e-145">Mailing and physical addresses</span></span>
- <span data-ttu-id="e351e-146">Адреса электронной почты</span><span class="sxs-lookup"><span data-stu-id="e351e-146">Email addresses</span></span>
- <span data-ttu-id="e351e-147">Веб-сайты</span><span class="sxs-lookup"><span data-stu-id="e351e-147">Websites</span></span>
   
  ![Пример извлечения данных визитной карточки.](images/biz-card-extraction.png)

<span data-ttu-id="e351e-149">vCard (VCF-файл) с извлеченными контактной информацией также внедряется в страницу.</span><span class="sxs-lookup"><span data-stu-id="e351e-149">A vCard (.VCF file) with the extracted contact information is also embedded in the page. The vCard is a convenient way to get the contact information when retrieving page HTML content.</span></span> <span data-ttu-id="e351e-150">vCard — это удобный способ получения контактной информации при получении HTML-контента страницы.</span><span class="sxs-lookup"><span data-stu-id="e351e-150">A vCard (.VCF file) with the extracted contact information is also embedded in the page. The vCard is a convenient way to get the contact information when retrieving page HTML content.</span></span>

### <a name="common-scenarios-for-business-card-extractions"></a><span data-ttu-id="e351e-151">Стандартные сценарии извлечения элементов визитных карточек</span><span class="sxs-lookup"><span data-stu-id="e351e-151">Common scenarios for business card extractions</span></span>

<span data-ttu-id="e351e-152">**Извлечение данных визитной карточки и отрисовка ее изображения**</span><span class="sxs-lookup"><span data-stu-id="e351e-152">**Extract business card information, and also render the business card image**</span></span>

<span data-ttu-id="e351e-153">Укажите метод `extract.businesscard` и резервное действие `none`.</span><span class="sxs-lookup"><span data-stu-id="e351e-153">Specify the `extract.businesscard` method and the `none` fallback.</span></span> <span data-ttu-id="e351e-154">Кроме того, отправьте элемент `img` с атрибутом `src`, который также ссылается на изображение.</span><span class="sxs-lookup"><span data-stu-id="e351e-154">Also send an `img` element with the `src` attribute that also references the image.</span></span> <span data-ttu-id="e351e-155">Если API не может извлечь какой-либо контент, он отрисовывает только изображение визитной карточки.</span><span class="sxs-lookup"><span data-stu-id="e351e-155">If the API is unable to extract any content, it renders the business card image only.</span></span>

```html 
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard"
    data-render-fallback="none">
</div>
<img src="name:scanned-card-image" />
```


<span data-ttu-id="e351e-156">**Извлечение данных визитной карточки и отрисовка ее изображения только при неудачном извлечении**</span><span class="sxs-lookup"><span data-stu-id="e351e-156">**Extract business card information, and render the business card image only if the extraction fails**</span></span>

<span data-ttu-id="e351e-157">Укажите метод `extract.businesscard` и используйте резервное действие по умолчанию `render`.</span><span class="sxs-lookup"><span data-stu-id="e351e-157">Specify the `extract.businesscard` method and use the default `render` fallback.</span></span> <span data-ttu-id="e351e-158">Если API не может извлечь какой-либо контент, он отрисовывает изображение визитной карточки.</span><span class="sxs-lookup"><span data-stu-id="e351e-158">If the API is unable to extract any content, it renders the business card image instead.</span></span>

```html
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard">
</div>
```
 
<span data-ttu-id="e351e-159">При извлечении данных визитной карточки изображение отправляется в виде именованной части в составном запросе.</span><span class="sxs-lookup"><span data-stu-id="e351e-159">For business card extractions, the image is sent as a named part in a multipart request.</span></span> <span data-ttu-id="e351e-160">Примеры отправки изображения в запросе см. в статье [Добавление изображений и файлов](onenote_images_files.md).</span><span class="sxs-lookup"><span data-stu-id="e351e-160">See Capture photos and images  for examples that show how to send an image in a create-page request.</span></span>


<a name="recipe"></a>
## <a name="recipe-extractions"></a><span data-ttu-id="e351e-161">Извлечение рецептов</span><span class="sxs-lookup"><span data-stu-id="e351e-161">Recipe extractions</span></span>

<span data-ttu-id="e351e-162">На основе URL-адреса рецепта API OneNote пытается найти и отобразить указанные ниже сведения.</span><span class="sxs-lookup"><span data-stu-id="e351e-162">The onnvshort API tries to find and  render the following information based on a recipe's URL.</span></span>

- <span data-ttu-id="e351e-163">Изображение главного имиджевого баннера</span><span class="sxs-lookup"><span data-stu-id="e351e-163">Hero image</span></span>
- <span data-ttu-id="e351e-164">Оценка</span><span class="sxs-lookup"><span data-stu-id="e351e-164">Rating</span></span>
- <span data-ttu-id="e351e-165">ингредиенты;</span><span class="sxs-lookup"><span data-stu-id="e351e-165">Ingredients</span></span>
- <span data-ttu-id="e351e-166">Инструкции</span><span class="sxs-lookup"><span data-stu-id="e351e-166">Instructions</span></span>
- <span data-ttu-id="e351e-167">время подготовки, приготовления и общее;</span><span class="sxs-lookup"><span data-stu-id="e351e-167">Prep, cook, and total times</span></span>
- <span data-ttu-id="e351e-168">Сервировка</span><span class="sxs-lookup"><span data-stu-id="e351e-168">Servings</span></span>

   ![Пример извлечения рецепта](images/recipe-extraction.png)

<span data-ttu-id="e351e-170">API оптимизирован для работы с рецептами со многих популярных сайтов, например *Allrecipes.com*, *FoodNetwork.com* и *SeriousEats.com*.</span><span class="sxs-lookup"><span data-stu-id="e351e-170">The API is optimized for recipes from many popular sites such as Allrecipes.com, FoodNetwork.com, and SeriousEats.com.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="e351e-171">Стандартные сценарии извлечения рецептов</span><span class="sxs-lookup"><span data-stu-id="e351e-171">Common scenarios for recipe extractions</span></span>

<span data-ttu-id="e351e-172">**Извлечение рецепта и отображение снимка веб-страницы с рецептом**</span><span class="sxs-lookup"><span data-stu-id="e351e-172">**Extract recipe information, and also render a snapshot of the recipe webpage**</span></span>

<span data-ttu-id="e351e-173">Укажите метод `extract.recipe` и резервное действие `none`.</span><span class="sxs-lookup"><span data-stu-id="e351e-173">Specify the `extract.recipe` method and the `none` fallback.</span></span> <span data-ttu-id="e351e-174">Кроме того, отправьте элемент `img` с атрибутом `data-render-src`, в качестве значения которого используется URL-адрес рецепта.</span><span class="sxs-lookup"><span data-stu-id="e351e-174">Also send an `img` element with the `data-render-src` attribute set to the recipe URL.</span></span> <span data-ttu-id="e351e-175">Если API не может извлечь какой-либо контент, он отображает только снимок веб-страницы с рецептом.</span><span class="sxs-lookup"><span data-stu-id="e351e-175">If the API is unable to extract any content, it renders a snapshot of the recipe webpage only.</span></span>

<span data-ttu-id="e351e-176">Потенциально этот сценарий дает максимальное количество сведений, так как на веб-странице может быть дополнительная информация, например отзывы и предложения клиентов.</span><span class="sxs-lookup"><span data-stu-id="e351e-176">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="http://allrecipes.com/recipe/guacamole/"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<img data-render-src="http://allrecipes.com/recipe/guacamole/" />
```
 

<span data-ttu-id="e351e-177">**Извлечение рецепта и отображение снимка веб-страницы с рецептом только в случае неудачного извлечения**</span><span class="sxs-lookup"><span data-stu-id="e351e-177">**Extract recipe information, and render a snapshot of the recipe webpage only if the extraction fails**</span></span>

<span data-ttu-id="e351e-178">Укажите метод `extract.recipe` и используйте резервное действие по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e351e-178">Specify the `extract.recipe` method and use the default render fallback.</span></span> <span data-ttu-id="e351e-179">Если API не может извлечь какой-либо контент, он отображает снимок веб-страницы с рецептом.</span><span class="sxs-lookup"><span data-stu-id="e351e-179">If the API is unable to extract any content, it renders a snapshot of the recipe webpage instead.</span></span>

```html  
<div
    data-render-src="http://www.foodnetwork.com/recipes/alton-brown/creme-brulee-recipe.html"
    data-render-method="extract.recipe">
</div>
```


<span data-ttu-id="e351e-180">**Извлечение рецепта и отображение ссылки на рецепт**</span><span class="sxs-lookup"><span data-stu-id="e351e-180">**Extract recipe information, and also render a link to the recipe**</span></span>

<span data-ttu-id="e351e-181">Укажите метод `extract.recipe` и резервное действие `none`.</span><span class="sxs-lookup"><span data-stu-id="e351e-181">Specify the `extract.recipe` method and the `none` fallback.</span></span> <span data-ttu-id="e351e-182">Кроме того, отправьте элемент `a` с атрибутом `src`, в качестве значения которого задан URL-адрес рецепта (вы также можете отправить любую информацию, которую необходимо добавить на страницу).</span><span class="sxs-lookup"><span data-stu-id="e351e-182">Extract recipe information, and also render  a link to the recipeSpecify the extract.recipe`a` method and the none`src` fallback. Also send an a element with the src  attribute set to the recipe URL (or you can send any other information you want to add to the page). If the API is unable to extract any content, only the recipe link is rendered.</span></span> <span data-ttu-id="e351e-183">Если API не может извлечь какой-либо контент, отображается только ссылка на рецепт.</span><span class="sxs-lookup"><span data-stu-id="e351e-183">If the API is unable to extract any content, only the recipe link is rendered.</span></span>

```html  
<div
    data-render-src="http://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<a href="http://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html">Recipe URL</a>
``` 


<a name="product"></a>
## <a name="product-listing-extractions"></a><span data-ttu-id="e351e-184">Извлечение описания товара</span><span class="sxs-lookup"><span data-stu-id="e351e-184">Product listing extractions</span></span>

- <span data-ttu-id="e351e-185">Название</span><span class="sxs-lookup"><span data-stu-id="e351e-185">Title</span></span>
- <span data-ttu-id="e351e-186">Оценка</span><span class="sxs-lookup"><span data-stu-id="e351e-186">Rating</span></span>
- <span data-ttu-id="e351e-187">первичное изображение;</span><span class="sxs-lookup"><span data-stu-id="e351e-187">Primary image</span></span>
- <span data-ttu-id="e351e-188">Описание</span><span class="sxs-lookup"><span data-stu-id="e351e-188">Description</span></span>
- <span data-ttu-id="e351e-189">Возможности</span><span class="sxs-lookup"><span data-stu-id="e351e-189">Features</span></span>
- <span data-ttu-id="e351e-190">Спецификации</span><span class="sxs-lookup"><span data-stu-id="e351e-190">Specifications</span></span></td>

  ![Пример извлечения описания товара.](images/product-extraction.png)

<span data-ttu-id="e351e-192">API оптимизирован для работы с товарами со многих популярных сайтов, например *Amazon.com* и *HomeDepot.com*.</span><span class="sxs-lookup"><span data-stu-id="e351e-192">The API is optimized for products from many popular sites such as Amazon.com, HomeDepot.com, and Sears.com.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="e351e-193">Стандартные сценарии извлечения рецептов</span><span class="sxs-lookup"><span data-stu-id="e351e-193">Common scenarios for recipe extractions</span></span>

<span data-ttu-id="e351e-194">**Извлечение информации о товаре и отображение снимка веб-страницы товара**</span><span class="sxs-lookup"><span data-stu-id="e351e-194">**Extract product information, and also render a snapshot of the product webpage**</span></span>

<span data-ttu-id="e351e-195">Укажите метод `extract.product` и резервное действие `none`.</span><span class="sxs-lookup"><span data-stu-id="e351e-195">Specify the `extract.product` method and the `none` fallback.</span></span> <span data-ttu-id="e351e-196">Кроме того, отправьте элемент `img` с атрибутом `data-render-src`, в качестве значения которого используется URL-адрес страницы товара.</span><span class="sxs-lookup"><span data-stu-id="e351e-196">Also send an `img` element with the `data-render-src` attribute set to the product URL.</span></span> <span data-ttu-id="e351e-197">Если API не может извлечь какой-либо контент, он отображает только снимок веб-страницы товара.</span><span class="sxs-lookup"><span data-stu-id="e351e-197">If the API is unable to extract any content, it renders a snapshot of the product webpage only.</span></span>

<span data-ttu-id="e351e-198">Потенциально этот сценарий дает максимальное количество сведений, так как на веб-странице может быть дополнительная информация, например отзывы и предложения клиентов.</span><span class="sxs-lookup"><span data-stu-id="e351e-198">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="http://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<img data-render-src="http://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO" />
```


<span data-ttu-id="e351e-199">**Извлечение информации о товаре и отображение снимка веб-страницы с товаром только в случае неудачного извлечения**</span><span class="sxs-lookup"><span data-stu-id="e351e-199">**Extract product information, and render a snapshot of the product webpage only if the extraction fails**</span></span>

<span data-ttu-id="e351e-200">Укажите метод `extract.product` и используйте резервное действие по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e351e-200">Specify the `extract.product` method and use the default render fallback.</span></span> <span data-ttu-id="e351e-201">Если API не может извлечь какой-либо контент, он вместо этого отображает снимок веб-страницы товара.</span><span class="sxs-lookup"><span data-stu-id="e351e-201">If the API is unable to extract any content, it renders a snapshot of the product webpage instead.</span></span>

```html 
<div
    data-render-src="http://www.sears.com/craftsman-19hp-42-8221-turn-tight-174-hydrostatic-yard-tractor/p-07120381000P"
    data-render-method="extract.product">
</div>
```
 

<span data-ttu-id="e351e-202">**Извлечение информации о товаре и отображение ссылки на товар**</span><span class="sxs-lookup"><span data-stu-id="e351e-202">**Extract product information, and also render a link to the product**</span></span>

<span data-ttu-id="e351e-203">Укажите метод `extract.product` и резервное действие `none`.</span><span class="sxs-lookup"><span data-stu-id="e351e-203">Specify the `extract.product` method and the `none` fallback.</span></span> <span data-ttu-id="e351e-204">Кроме того, отправьте элемент `a` с атрибутом `src`, в качестве значения которого задан URL-адрес страницы товара (вы также можете отправить любую информацию, которую необходимо добавить на страницу).</span><span class="sxs-lookup"><span data-stu-id="e351e-204">Extract product information, and also render  a link to the productSpecify the extract.product`a` method and the none`src` fallback. Also send an a element with the src  attribute set to the product URL (or you can send any other information you want to add to the page). If the API is unable to extract any content, only the page link is rendered.</span></span> <span data-ttu-id="e351e-205">Если API не может извлечь какой-либо контент, отображается только ссылка на страницу.</span><span class="sxs-lookup"><span data-stu-id="e351e-205">If the API is unable to extract any content, only the page link is rendered.</span></span>

```html 
<div
    data-render-src="http://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<a href="http://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001">Product URL</a>
```


<a name="unknown"></a> 
## <a name="unknown-content-type-extractions"></a><span data-ttu-id="e351e-206">Извлечение содержимого неизвестного типа</span><span class="sxs-lookup"><span data-stu-id="e351e-206">Unknown content type extractions</span></span>

<span data-ttu-id="e351e-207">Если вы не знаете тип контента (визитная карточка, рецепт или товар), который вы отправляете, вы можете использовать неполный метод `extract` и разрешить API OneNote автоматически определять тип контента.</span><span class="sxs-lookup"><span data-stu-id="e351e-207">If you don't know the content type (business card, recipe, or product) that you're sending,   you can use the unqualified extract method and let the onnvshort API automatically detect the type. You might want to do this if your app sends different capture types.</span></span> <span data-ttu-id="e351e-208">Вы можете сделать это, если ваше приложение отправляет изображения различных типов.</span><span class="sxs-lookup"><span data-stu-id="e351e-208">You might want to do this if your app sends different capture types.</span></span>

> <span data-ttu-id="e351e-209">**Примечание.** Если вы не знаете тип контента, который вы отправляете, используйте метод `extract.businesscard`, `extract.recipe` или `extract.product`.</span><span class="sxs-lookup"><span data-stu-id="e351e-209">**Note:** If you do know the content type that you're sending, you should use the `extract.businesscard`, `extract.recipe`, or `extract.product` method.</span></span> <span data-ttu-id="e351e-210">В некоторых случаях это позволяет оптимизировать результаты извлечения.</span><span class="sxs-lookup"><span data-stu-id="e351e-210">In some cases, this can help to optimize the extraction results.</span></span>
 
### <a name="common-scenarios-for-unknown-extractions"></a><span data-ttu-id="e351e-211">Стандартные сценарии извлечения контента неизвестного типа</span><span class="sxs-lookup"><span data-stu-id="e351e-211">Common  scenarios for article extractions</span></span>

<span data-ttu-id="e351e-212">**Отправка изображения или URL-адреса и отображение предоставленного изображения или снимка веб-страницы при неудачном извлечении**</span><span class="sxs-lookup"><span data-stu-id="e351e-212">**Send an image or a URL, and render the supplied image or a snapshot of the webpage if the extraction fails**</span></span>

<span data-ttu-id="e351e-213">Укажите метод `extract`, чтобы API автоматически определял тип контента, и используйте резервное действие по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e351e-213">Specify the `extract` method so the API automatically detects the content type, and use the default render fallback.</span></span> <span data-ttu-id="e351e-214">Если API не может извлечь какой-либо контент, он отображает предоставленное изображение или снимок веб-страницы.</span><span class="sxs-lookup"><span data-stu-id="e351e-214">If the API is unable to extract any content, it renders the supplied image or snapshot of the webpage instead.</span></span>

```html 
<div
    data-render-src="some image or url"
    data-render-method="extract">
</div>
```


<a name="request-response-info"></a>
## <a name="response-information"></a><span data-ttu-id="e351e-215">Информация в ответе</span><span class="sxs-lookup"><span data-stu-id="e351e-215">Response information</span></span>

| <span data-ttu-id="e351e-216">Данные в ответе</span><span class="sxs-lookup"><span data-stu-id="e351e-216">Response data</span></span> | <span data-ttu-id="e351e-217">Описание</span><span class="sxs-lookup"><span data-stu-id="e351e-217">Description</span></span> |  
|------|------|  
| <span data-ttu-id="e351e-218">код успешного завершения действия;</span><span class="sxs-lookup"><span data-stu-id="e351e-218">Success code</span></span> | <span data-ttu-id="e351e-219">Код состояния HTTP 201 при успешном выполнении запроса POST и код состояния HTTP 204 при успешном выполнении запроса PATCH.</span><span class="sxs-lookup"><span data-stu-id="e351e-219">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="e351e-220">Ошибки</span><span class="sxs-lookup"><span data-stu-id="e351e-220">Errors</span></span>| <span data-ttu-id="e351e-221">Дополнительные сведения об ошибках OneNote, которые может возвращать Microsoft Graph, см. в статье [Коды ошибок для API OneNote в Microsoft Graph](onenote_error_codes.md).</span><span class="sxs-lookup"><span data-stu-id="e351e-221">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  


<a name="permissions"></a>
## <a name="permissions"></a><span data-ttu-id="e351e-222">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e351e-222">Permissions</span></span>

<span data-ttu-id="e351e-223">Чтобы можно было создавать или изменять страницы OneNote, вам придется запросить соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="e351e-223">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="e351e-224">Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="e351e-224">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="e351e-225">**Разрешения для _запросов POST со страницами_**</span><span class="sxs-lookup"><span data-stu-id="e351e-225">**Permissions for _POST pages_**</span></span>

- <span data-ttu-id="e351e-226">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="e351e-226">Notes.Create</span></span>
- <span data-ttu-id="e351e-227">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e351e-227">Notes.ReadWrite</span></span>
- <span data-ttu-id="e351e-228">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e351e-228">Notes.ReadWrite.All</span></span>  

<span data-ttu-id="e351e-229">**Разрешения для _запросов PATCH со страницами_**</span><span class="sxs-lookup"><span data-stu-id="e351e-229">**Permissions for _PATCH pages_**</span></span>

- <span data-ttu-id="e351e-230">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e351e-230">Notes.ReadWrite</span></span>
- <span data-ttu-id="e351e-231">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e351e-231">Notes.ReadWrite.All</span></span>

<span data-ttu-id="e351e-232">Дополнительные сведения о разрешениях и принципе их работы см. в [справочнике по разрешениям Microsoft Graph](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e351e-232">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions_reference.md).</span></span>


<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="e351e-233">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="e351e-233">Additional resources</span></span>

- [<span data-ttu-id="e351e-234">Создание страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="e351e-234">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="e351e-235">Обновление содержимого страницы OneNote</span><span class="sxs-lookup"><span data-stu-id="e351e-235">Update OneNote page content</span></span>](onenote_update_page.md)
- [<span data-ttu-id="e351e-236">Добавление изображений и файлов</span><span class="sxs-lookup"><span data-stu-id="e351e-236">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="e351e-237">Интеграция с OneNote</span><span class="sxs-lookup"><span data-stu-id="e351e-237">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="e351e-238">Блог разработчиков OneNote</span><span class="sxs-lookup"><span data-stu-id="e351e-238">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="e351e-239">Вопросы разработки OneNote на сайте Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="e351e-239">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="e351e-240">Репозитории GitHub OneNote</span><span class="sxs-lookup"><span data-stu-id="e351e-240">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  

