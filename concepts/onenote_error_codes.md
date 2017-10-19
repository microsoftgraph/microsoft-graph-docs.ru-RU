# <a name="error-codes-for-onenote-apis-in-microsoft-graph"></a><span data-ttu-id="793a1-101">Коды ошибок для API OneNote в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="793a1-101">Error codes for OneNote APIs in Microsoft Graph</span></span>

<span data-ttu-id="793a1-102">В этой статье описываются коды ошибок, возвращаемые API OneNote в Microsoft Graph при сбоях запросов, отправляемых через API.</span><span class="sxs-lookup"><span data-stu-id="793a1-102">This topic describes error and warning codes that are returned by the onnvshort API whenever a request sent through the API fails.</span></span>

## <a name="error-response-example"></a><span data-ttu-id="793a1-103">Пример ответа об ошибке</span><span class="sxs-lookup"><span data-stu-id="793a1-103">Error response example</span></span>
<span data-ttu-id="793a1-104">Если при отправке запроса возникает ошибка, API OneNote перестает выполнять запрос и возвращает ответ об ошибке в виде объекта JSON.</span><span class="sxs-lookup"><span data-stu-id="793a1-104">When your request generates an error, the OneNote API stops performing the request and returns an error response as a JSON object.</span></span> <span data-ttu-id="793a1-105">Ответ об ошибке содержит соответствующий код ошибки, сообщение и ссылку на соответствующий раздел этой статьи.</span><span class="sxs-lookup"><span data-stu-id="793a1-105">An error response contains the associated error code, a message, and a link to the appropriate section of this article.</span></span> <span data-ttu-id="793a1-106">В приведенном ниже примере показано, как выглядит ответ об ошибке.</span><span class="sxs-lookup"><span data-stu-id="793a1-106">The following example shows how an error response looks.</span></span>

```json
{
   "error":{
      "code":"10002",
      "message":"The service is currently unavailable. Please try again later.",
      "innerError": {
        "requestId": "request-id",
        "date": "date-time"
      }
   }
}
```

<span data-ttu-id="793a1-107">Дополнительные сведения об ошибках Microsoft Graph см. в статье [Сообщения об ошибках и типы ресурсов ошибок Microsoft Graph](errors.md).</span><span class="sxs-lookup"><span data-stu-id="793a1-107">For more information about Microsoft Graph errors, see [Microsoft Graph error responses and resource types](errors.md).</span></span>

## <a name="codes-from-10001-to-19999"></a><span data-ttu-id="793a1-108">Коды от 10001 до 19999</span><span class="sxs-lookup"><span data-stu-id="793a1-108">Codes from 10001 to 19999</span></span>
<span data-ttu-id="793a1-109">Служба работает с ошибками или отправляет информацию в приложение.</span><span class="sxs-lookup"><span data-stu-id="793a1-109">The service is having problems or is sending information to the application.</span></span>

### <a name="10001"></a><span data-ttu-id="793a1-110">10001</span><span class="sxs-lookup"><span data-stu-id="793a1-110">10001</span></span>
<span data-ttu-id="793a1-111">Произошла непредвиденная ошибка, и запрос не выполнен.</span><span class="sxs-lookup"><span data-stu-id="793a1-111">An unexpected error occurred and the request failed.</span></span>

### <a name="10002"></a><span data-ttu-id="793a1-112">10002</span><span class="sxs-lookup"><span data-stu-id="793a1-112">10002</span></span>
<span data-ttu-id="793a1-113">Служба в настоящее время недоступна.</span><span class="sxs-lookup"><span data-stu-id="793a1-113">The service is not currently available.</span></span>

### <a name="10003"></a><span data-ttu-id="793a1-114">10003</span><span class="sxs-lookup"><span data-stu-id="793a1-114">10003</span></span>
<span data-ttu-id="793a1-115">Учетная запись текущего пользователя превысила максимальное число активных запросов.</span><span class="sxs-lookup"><span data-stu-id="793a1-115">The current user’s account has exceeded the maximum number of active requests. Your app will have to repeat the request.</span></span> <span data-ttu-id="793a1-116">Приложению придется повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="793a1-116">Your app will have to repeat the request.</span></span>

### <a name="10004"></a><span data-ttu-id="793a1-117">10004</span><span class="sxs-lookup"><span data-stu-id="793a1-117">10004</span></span>
<span data-ttu-id="793a1-118">Служба не может создать страницу в запрашиваемом разделе, так как раздел защищен паролем.</span><span class="sxs-lookup"><span data-stu-id="793a1-118">The service can’t create a page in the requested section because that section is protected by a password.</span></span>

### <a name="10005"></a><span data-ttu-id="793a1-119">10005</span><span class="sxs-lookup"><span data-stu-id="793a1-119">10005</span></span>
<span data-ttu-id="793a1-120">В запросе превышено максимальное количество тегов изображений, в которых атрибут **data-render-src** содержит PDF-файл.</span><span class="sxs-lookup"><span data-stu-id="793a1-120">The request contains more than the maximum number of image tags in which the **data-render-src** attribute contains a PDF. See  for more information.</span></span> <span data-ttu-id="793a1-121">См. статью [Добавление изображений и файлов](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files).</span><span class="sxs-lookup"><span data-stu-id="793a1-121">See [Add images and files](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files).</span></span>

### <a name="10006"></a><span data-ttu-id="793a1-122">10006</span><span class="sxs-lookup"><span data-stu-id="793a1-122">10006</span></span>
<span data-ttu-id="793a1-123">API OneNote не удалось создать страницу в указанном разделе, потому что раздел поврежден.</span><span class="sxs-lookup"><span data-stu-id="793a1-123">The oncshort API was unable to create a page in the specified section because that section is corrupt.</span></span>

### <a name="10007"></a><span data-ttu-id="793a1-124">10007</span><span class="sxs-lookup"><span data-stu-id="793a1-124">10007</span></span>
<span data-ttu-id="793a1-p104">Сервер слишком занят, чтобы обработать входящий запрос в данный момент. Повторите попытку позже.</span><span class="sxs-lookup"><span data-stu-id="793a1-p104">The server is too busy to handle the incoming request at this moment. Please try again later.</span></span>

### <a name="10008"></a><span data-ttu-id="793a1-127">10008</span><span class="sxs-lookup"><span data-stu-id="793a1-127">10008</span></span>
<span data-ttu-id="793a1-128">Одна или несколько библиотек документов в хранилище OneDrive пользователя или группы содержит более 5000 элементов OneNote (записных книжек, разделов, групп разделов), и к ней невозможно отправлять запросы с помощью API.</span><span class="sxs-lookup"><span data-stu-id="793a1-128">One or more of the document libraries on the user or group's OneDrive contains more than 5000 OneNote items (notebooks, sections, section groups), and cannot be queried using the API.</span></span> <span data-ttu-id="793a1-129">Убедитесь, что ни одна из библиотек документов пользователей и групп не содержит более 5000 элементов OneNote.</span><span class="sxs-lookup"><span data-stu-id="793a1-129">Please make sure that none of the user or group's document libraries contains more than 5000 OneNote items.</span></span> <span data-ttu-id="793a1-130">Указания по устранению этой проблемы см. в [блоге разработчиков OneNote](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/).</span><span class="sxs-lookup"><span data-stu-id="793a1-130">See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10012"></a><span data-ttu-id="793a1-131">10012</span><span class="sxs-lookup"><span data-stu-id="793a1-131">10012</span></span>
<span data-ttu-id="793a1-132">Не удается создать или обновить объект, так как в библиотеке, содержащей записную книжку, требуется получать элементы для изменения, прежде чем редактировать их.</span><span class="sxs-lookup"><span data-stu-id="793a1-132">Unable to create or update the entity because the library that contains the notebook requires items to be checked out before they can be edited.</span></span> <span data-ttu-id="793a1-133">Дополнительные сведения см. в статье https://support.office.com/ru-ru/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7.</span><span class="sxs-lookup"><span data-stu-id="793a1-133">For more information, see https://support.office.com/en-us/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7.</span></span>

<span data-ttu-id="793a1-134">Отмените обязательное извлечение для этой библиотеки или переместите записную книжку.</span><span class="sxs-lookup"><span data-stu-id="793a1-134">Either remove the check-out requirement from the library, or move the notebook.</span></span>

### <a name="10013"></a><span data-ttu-id="793a1-135">10013</span><span class="sxs-lookup"><span data-stu-id="793a1-135">10013</span></span>
<span data-ttu-id="793a1-136">Одна или несколько библиотек документов в хранилище OneDrive пользователя или группы содержит более 20 000 элементов и не может быть индексирована для запросов с помощью API.</span><span class="sxs-lookup"><span data-stu-id="793a1-136">One or more of the document libraries on the user or group's OneDrive contains more than 20,000 items and cannot be indexed for querying using the API.</span></span> <span data-ttu-id="793a1-137">Убедитесь, что ни одна из библиотек документов пользователей и групп не содержит более 20 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="793a1-137">Please make sure that none of the user or group's document libraries contains more than 20,000 items.</span></span> <span data-ttu-id="793a1-138">Указания по устранению этой проблемы см. в [блоге разработчиков OneNote](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/).</span><span class="sxs-lookup"><span data-stu-id="793a1-138">See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10014"></a><span data-ttu-id="793a1-139">10014</span><span class="sxs-lookup"><span data-stu-id="793a1-139">10014</span></span>
<span data-ttu-id="793a1-140">В данный момент служба Azure Key Vault слишком занята для обработки входящего запроса.</span><span class="sxs-lookup"><span data-stu-id="793a1-140">The server is too busy to handle the incoming request at this moment. Please try again later.</span></span> <span data-ttu-id="793a1-141">Повторите попытку позже.</span><span class="sxs-lookup"><span data-stu-id="793a1-141">Please try again later.</span></span>

### <a name="10015"></a><span data-ttu-id="793a1-142">10015</span><span class="sxs-lookup"><span data-stu-id="793a1-142">10015</span></span>
<span data-ttu-id="793a1-143">В настоящее время среда SharePoint недоступна.</span><span class="sxs-lookup"><span data-stu-id="793a1-143">SharePoint is currently unavailable.</span></span> <span data-ttu-id="793a1-144">Повторите попытку позже.</span><span class="sxs-lookup"><span data-stu-id="793a1-144">Please try again later.</span></span>

### <a name="10016"></a><span data-ttu-id="793a1-145">10016</span><span class="sxs-lookup"><span data-stu-id="793a1-145">10016</span></span>
<span data-ttu-id="793a1-146">Библиотека документов в хранилище OneDrive пользователя или группы превысила пороговое количество уникальных областей безопасности.</span><span class="sxs-lookup"><span data-stu-id="793a1-146">Document library on the user or group’s OneDrive exceeded unique security scopes threshold limit.</span></span> <span data-ttu-id="793a1-147">Число уникальных областей безопасности для каждой библиотеки не может превышать 50 000.</span><span class="sxs-lookup"><span data-stu-id="793a1-147">The maximum number of unique security scopes set for a library cannot exceed 50,000.</span></span>

### <a name="10017"></a><span data-ttu-id="793a1-148">10017</span><span class="sxs-lookup"><span data-stu-id="793a1-148">10017</span></span>
<span data-ttu-id="793a1-149">Неправильный запрос.</span><span class="sxs-lookup"><span data-stu-id="793a1-149">Bad Request</span></span>

### <a name="19999"></a><span data-ttu-id="793a1-150">19999</span><span class="sxs-lookup"><span data-stu-id="793a1-150">19999</span></span>
<span data-ttu-id="793a1-151">Запрос не выполнен из-за неизвестной ошибки.</span><span class="sxs-lookup"><span data-stu-id="793a1-151">The request failed because an undetermined error occurred.</span></span>

## <a name="codes-from-20001-to-29999"></a><span data-ttu-id="793a1-152">Коды от 20001 до 29999</span><span class="sxs-lookup"><span data-stu-id="793a1-152">Codes from 20001 to 29999</span></span>
<span data-ttu-id="793a1-153">Код приложения допустил ошибку.</span><span class="sxs-lookup"><span data-stu-id="793a1-153">The application code has done something wrong.</span></span>

### <a name="20001"></a><span data-ttu-id="793a1-154">20001</span><span class="sxs-lookup"><span data-stu-id="793a1-154">20001</span></span>

<span data-ttu-id="793a1-155">В запросе отсутствует необходимый раздел Presentation.</span><span class="sxs-lookup"><span data-stu-id="793a1-155">The request is missing the required "Presentation" part.</span></span> <span data-ttu-id="793a1-156">Он должен быть только один.</span><span class="sxs-lookup"><span data-stu-id="793a1-156">Exactly one is required.</span></span> 

### <a name="20002"></a><span data-ttu-id="793a1-157">20002</span><span class="sxs-lookup"><span data-stu-id="793a1-157">20002</span></span>
<span data-ttu-id="793a1-158">Запрос содержит две или более части Presentation.</span><span class="sxs-lookup"><span data-stu-id="793a1-158">The request contains two or more "Presentation" parts.</span></span> <span data-ttu-id="793a1-159">Он должен быть только один.</span><span class="sxs-lookup"><span data-stu-id="793a1-159">Exactly one is required.</span></span>

### <a name="20003"></a><span data-ttu-id="793a1-160">20003</span><span class="sxs-lookup"><span data-stu-id="793a1-160">20003</span></span>
<span data-ttu-id="793a1-161">В разделе Presentation допускаются только типы контента text/HTML и application/XHTML+XML.</span><span class="sxs-lookup"><span data-stu-id="793a1-161">The content type of the "Presentation" part can be only text/HTML or application/XHTML+XML.</span></span> 

### <a name="20004"></a><span data-ttu-id="793a1-162">20004</span><span class="sxs-lookup"><span data-stu-id="793a1-162">20004</span></span>
<span data-ttu-id="793a1-163">HTML-код раздела Presentation содержит тег image, в котором заданы свойства **src** и **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="793a1-163">The "Presentation" part HTML contains an image tag with both the **src** and the **data-render-src** properties set.</span></span> <span data-ttu-id="793a1-164">API проигнорирует свойство **src** и будет использовать свойство **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="793a1-164">The API will ignore the **src** property and use the **data-render-src** property.</span></span> 

### <a name="20005"></a><span data-ttu-id="793a1-165">20005</span><span class="sxs-lookup"><span data-stu-id="793a1-165">20005</span></span>
<span data-ttu-id="793a1-166">URI запроса слишком длинный.</span><span class="sxs-lookup"><span data-stu-id="793a1-166">The request URI is too long.</span></span> <span data-ttu-id="793a1-167">Максимальный размер URI (включая все параметры и данные) составляет 16 КБ или 16 384 символов.</span><span class="sxs-lookup"><span data-stu-id="793a1-167">The request URI is too long. The maximum size of the URI (including all parameters and data) is 16 kb or 16,384 characters.</span></span>

### <a name="20006"></a><span data-ttu-id="793a1-168">20006</span><span class="sxs-lookup"><span data-stu-id="793a1-168">20006</span></span>
<span data-ttu-id="793a1-169">HTML-код раздела Presentation содержит тег image, в котором не заданы свойства src и **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="793a1-169">The “Presentation” part HTML contains an image tag with neither the **src** nor the data-render-src properties set. The API will ignore the image tag. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> <span data-ttu-id="793a1-170">API проигнорирует тег **image**.</span><span class="sxs-lookup"><span data-stu-id="793a1-170">The API will ignore the **image** tag.</span></span> 

### <a name="20007"></a><span data-ttu-id="793a1-171">20007</span><span class="sxs-lookup"><span data-stu-id="793a1-171">20007</span></span>
<span data-ttu-id="793a1-172">HTML-код раздела Presentation содержит строку даты и времени создания, которая не соответствует ни одному из допустимых форматов.</span><span class="sxs-lookup"><span data-stu-id="793a1-172">The “Presentation” part HTML contains a created date/time string that does not match any of the allowed formats. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> 

### <a name="20008"></a><span data-ttu-id="793a1-173">20008</span><span class="sxs-lookup"><span data-stu-id="793a1-173">20008</span></span>
<span data-ttu-id="793a1-174">Размер запроса превышает допустимый.</span><span class="sxs-lookup"><span data-stu-id="793a1-174">The size of the document is too large.</span></span> 

### <a name="20009"></a><span data-ttu-id="793a1-175">20009</span><span class="sxs-lookup"><span data-stu-id="793a1-175">20009</span></span>
<span data-ttu-id="793a1-176">Запрос содержит разделы с повторяющимися именами.</span><span class="sxs-lookup"><span data-stu-id="793a1-176">The request contains parts with duplicate names.</span></span> <span data-ttu-id="793a1-177">Имена разделов должны быть уникальными.</span><span class="sxs-lookup"><span data-stu-id="793a1-177">Lookup table names must be unique.</span></span> 

### <a name="20010"></a><span data-ttu-id="793a1-178">20010</span><span class="sxs-lookup"><span data-stu-id="793a1-178">20010</span></span>
<span data-ttu-id="793a1-179">Для указанного типа контента не предоставлен заголовок Content-Disposition.</span><span class="sxs-lookup"><span data-stu-id="793a1-179">The Content-Disposition header was not supplied for the specified content type.</span></span> 

### <a name="20011"></a><span data-ttu-id="793a1-180">20011</span><span class="sxs-lookup"><span data-stu-id="793a1-180">20011</span></span>
<span data-ttu-id="793a1-181">Запрос содержит составные полезные данные неправильного формата.</span><span class="sxs-lookup"><span data-stu-id="793a1-181">The request contains a malformed multipart payload.</span></span> <span data-ttu-id="793a1-182">К возможным причинам этой ошибки относятся пустые строки, отсутствие последней строки, неправильно отформатированные разделители частей и т. д.</span><span class="sxs-lookup"><span data-stu-id="793a1-182">Problems could include missing blank lines, a missing last line, incorrectly formatted part separators, and so on.</span></span> <span data-ttu-id="793a1-183">Если вы создаете составное сообщение вручную, внимательно проверьте логику или используйте стороннюю библиотеку.</span><span class="sxs-lookup"><span data-stu-id="793a1-183">If you're building the multipart message by hand, carefully check the logic, or consider using a third-party library.</span></span> 

### <a name="20012"></a><span data-ttu-id="793a1-184">20012</span><span class="sxs-lookup"><span data-stu-id="793a1-184">20012</span></span>
<span data-ttu-id="793a1-185">В запросе не предоставлен тип контента для указанной части.</span><span class="sxs-lookup"><span data-stu-id="793a1-185">The request doesn't supply a content type for the specified part.</span></span> 
### <a name="20013"></a><span data-ttu-id="793a1-186">20013</span><span class="sxs-lookup"><span data-stu-id="793a1-186">20013</span></span>
<span data-ttu-id="793a1-187">В запросе не предоставлены заголовки Content-Type и Content-Disposition для указанной части.</span><span class="sxs-lookup"><span data-stu-id="793a1-187">The request doesn’t supply Content-Type and Content-Disposition headers for the specified part.</span></span> 

### <a name="20014"></a><span data-ttu-id="793a1-188">20014</span><span class="sxs-lookup"><span data-stu-id="793a1-188">20014</span></span>
<span data-ttu-id="793a1-189">Длина части составного сообщения превышает максимальную (25 МБ).</span><span class="sxs-lookup"><span data-stu-id="793a1-189">The length of a part in the multi-part message exceeds the maximum size of 25 MB. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> 

### <a name="20015"></a><span data-ttu-id="793a1-190">20015</span><span class="sxs-lookup"><span data-stu-id="793a1-190">20015</span></span>
<span data-ttu-id="793a1-191">Количество частей составного сообщения превышает максимальное (500).</span><span class="sxs-lookup"><span data-stu-id="793a1-191">The count of parts in the multi-part message exceeds the limit of 500. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> 

### <a name="20016"></a><span data-ttu-id="793a1-192">20016</span><span class="sxs-lookup"><span data-stu-id="793a1-192">20016</span></span>
<span data-ttu-id="793a1-193">Длина составного сообщения превышает максимальную (75 МБ).</span><span class="sxs-lookup"><span data-stu-id="793a1-193">The length of the multi-part message exceeds the limit of 75 MB. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> 

### <a name="20017"></a><span data-ttu-id="793a1-194">20017</span><span class="sxs-lookup"><span data-stu-id="793a1-194">20017</span></span>
<span data-ttu-id="793a1-195">Неправильный формат MIME электронного сообщения.</span><span class="sxs-lookup"><span data-stu-id="793a1-195">The email MIME was malformed.</span></span> 

### <a name="20018"></a><span data-ttu-id="793a1-196">20018</span><span class="sxs-lookup"><span data-stu-id="793a1-196">20018</span></span>
<span data-ttu-id="793a1-197">Неправильный формат MIME или элемента ICal для собрания.</span><span class="sxs-lookup"><span data-stu-id="793a1-197">The meeting MIME or ICal was malformed.</span></span> 

### <a name="20019"></a><span data-ttu-id="793a1-198">20019</span><span class="sxs-lookup"><span data-stu-id="793a1-198">20019</span></span>
<span data-ttu-id="793a1-199">Элемент ICal не найден.</span><span class="sxs-lookup"><span data-stu-id="793a1-199">No ICal was found.</span></span> 

### <a name="20020"></a><span data-ttu-id="793a1-200">20020</span><span class="sxs-lookup"><span data-stu-id="793a1-200">20020</span></span>
<span data-ttu-id="793a1-201">В теле запроса обнаружен объект JSON неправильного формата.</span><span class="sxs-lookup"><span data-stu-id="793a1-201">Encountered malformed Json in request body.</span></span> 

### <a name="20100"></a><span data-ttu-id="793a1-202">20100</span><span class="sxs-lookup"><span data-stu-id="793a1-202">20100</span></span>
<span data-ttu-id="793a1-203">Ошибка синтаксиса запроса.</span><span class="sxs-lookup"><span data-stu-id="793a1-203">Something is wrong with the syntax of your request.</span></span> 
### <a name="20101"></a><span data-ttu-id="793a1-204">20101</span><span class="sxs-lookup"><span data-stu-id="793a1-204">20101</span></span>
<span data-ttu-id="793a1-205">Запрашиваемое свойство не существует.</span><span class="sxs-lookup"><span data-stu-id="793a1-205">The property that you requested doesn’t exist.</span></span>

### <a name="20102"></a><span data-ttu-id="793a1-206">20102</span><span class="sxs-lookup"><span data-stu-id="793a1-206">20102</span></span>
<span data-ttu-id="793a1-207">Запрашиваемый ресурс не существует.</span><span class="sxs-lookup"><span data-stu-id="793a1-207">You requested a resource that doesn’t exist.</span></span>

### <a name="20103"></a><span data-ttu-id="793a1-208">20103</span><span class="sxs-lookup"><span data-stu-id="793a1-208">20103</span></span>
<span data-ttu-id="793a1-209">Оператор **expand** не поддерживается для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="793a1-209">The **expand** query is not supported for this request.</span></span> <span data-ttu-id="793a1-210">См. раздел [Поддерживаемые параметры строки запроса OData](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-get-content#query-options).</span><span class="sxs-lookup"><span data-stu-id="793a1-210">Supported OData query string options</span></span>

### <a name="20104"></a><span data-ttu-id="793a1-211">20104</span><span class="sxs-lookup"><span data-stu-id="793a1-211">20104 (SectionNameInvalidChar)</span></span>
<span data-ttu-id="793a1-212">Параметр запроса **pagelevel** поддерживается только для запросов к коллекции страниц в разделе или конкретной страницы.</span><span class="sxs-lookup"><span data-stu-id="793a1-212">The **pagelevel** query option is supported only when querying for the pages collection in a section or for a specific page. For example:</span></span> <span data-ttu-id="793a1-213">Например:</span><span class="sxs-lookup"><span data-stu-id="793a1-213">For example:</span></span>  

```http
GET ../sections/{id}/pages?pagelevel=true
GET ../pages/{id}?pagelevel=true
```

### <a name="20106"></a><span data-ttu-id="793a1-214">20106</span><span class="sxs-lookup"><span data-stu-id="793a1-214">20106</span></span>
<span data-ttu-id="793a1-215">Запрос содержит неподдерживаемый оператор.</span><span class="sxs-lookup"><span data-stu-id="793a1-215">Your request contains a query operator that is not supported. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> 

### <a name="20108"></a><span data-ttu-id="793a1-216">20108</span><span class="sxs-lookup"><span data-stu-id="793a1-216">20108</span></span>
<span data-ttu-id="793a1-217">Запрос содержит неподдерживаемые параметры запроса OData.</span><span class="sxs-lookup"><span data-stu-id="793a1-217">Your request contains unsupported OData query parameters.</span></span>

### <a name="20109"></a><span data-ttu-id="793a1-218">20109</span><span class="sxs-lookup"><span data-stu-id="793a1-218">20109</span></span>
<span data-ttu-id="793a1-219">Полезные данные в PATCH-запросе неправильно построены.</span><span class="sxs-lookup"><span data-stu-id="793a1-219">The payload in the PATCH request is not constructed correctly.</span></span>

### <a name="20110"></a><span data-ttu-id="793a1-220">20110</span><span class="sxs-lookup"><span data-stu-id="793a1-220">20110</span></span>
<span data-ttu-id="793a1-221">Для запросов на создание страниц с частями данных необходимо составное содержимое с разделом Presentation.</span><span class="sxs-lookup"><span data-stu-id="793a1-221">Page create requests with data parts require the content to be multi-part, with a “Presentation” part. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> 

### <a name="20111"></a><span data-ttu-id="793a1-222">20111</span><span class="sxs-lookup"><span data-stu-id="793a1-222">20111</span></span>
<span data-ttu-id="793a1-223">В запросе используется неподдерживаемая функция OData.</span><span class="sxs-lookup"><span data-stu-id="793a1-223">Your request uses an OData feature that isn’t supported.</span></span>

### <a name="20112"></a><span data-ttu-id="793a1-224">20112</span><span class="sxs-lookup"><span data-stu-id="793a1-224">20112</span></span>
<span data-ttu-id="793a1-225">Запрос содержит недопустимый идентификатор для целевой сущности записной книжки, группы разделов, раздела или страницы.</span><span class="sxs-lookup"><span data-stu-id="793a1-225">Your request contains an invalid ID for the target notebook, section group, section, or page entity.</span></span>

### <a name="20113"></a><span data-ttu-id="793a1-226">20113</span><span class="sxs-lookup"><span data-stu-id="793a1-226">20113</span></span>
<span data-ttu-id="793a1-227">Ресурс, заданный в запросе, был удален.</span><span class="sxs-lookup"><span data-stu-id="793a1-227">The resource specified in the request has been deleted.</span></span>

### <a name="20115"></a><span data-ttu-id="793a1-228">20115</span><span class="sxs-lookup"><span data-stu-id="793a1-228">20115</span></span>
<span data-ttu-id="793a1-229">Имя содержит недопустимые символы.</span><span class="sxs-lookup"><span data-stu-id="793a1-229">The name contains invalid characters.</span></span> <span data-ttu-id="793a1-230">Имя записной книжки не может содержать следующие символы: `? * \ / : < > | ' "`</span><span class="sxs-lookup"><span data-stu-id="793a1-230">The name contains invalid characters. A notebook name cannot contain any of the following characters: ?*\/:<>|'"</span></span>

### <a name="20117"></a><span data-ttu-id="793a1-231">20117</span><span class="sxs-lookup"><span data-stu-id="793a1-231">20117</span></span>
<span data-ttu-id="793a1-232">Элемент с таким именем уже существует в указанном месте.</span><span class="sxs-lookup"><span data-stu-id="793a1-232">An item with the name you specified already exists in the location that you specified.</span></span>

### <a name="20119"></a><span data-ttu-id="793a1-233">20119</span><span class="sxs-lookup"><span data-stu-id="793a1-233">20119</span></span>
<span data-ttu-id="793a1-234">HTML-код в разделе Presentation содержит атрибут **data-attachment**, который либо неправильно отформатирован либо содержит какие-либо из следующих недопустимых символов для имени файла: `\ / : * ? < > | "`.</span><span class="sxs-lookup"><span data-stu-id="793a1-234">The HTML in the 'Presentation' part contains a data-attachment attribute that either doesn’t have a valid format or includes one or more of these invalid characters for a file name: \/:*?<>|". The request substituted the value indicated in the error message.</span></span> <span data-ttu-id="793a1-235">Запрос заменил значение, указанное в сообщении об ошибке.</span><span class="sxs-lookup"><span data-stu-id="793a1-235">The request substituted the value indicated in the error message.</span></span>

### <a name="20120"></a><span data-ttu-id="793a1-236">20120</span><span class="sxs-lookup"><span data-stu-id="793a1-236">20120</span></span>
<span data-ttu-id="793a1-237">В запросе указан целевой объект операции PATCH, который не удается найти.</span><span class="sxs-lookup"><span data-stu-id="793a1-237">Your request specifies a PATCH target that can’t be located.</span></span>

### <a name="20121"></a><span data-ttu-id="793a1-238">20121</span><span class="sxs-lookup"><span data-stu-id="793a1-238">20121</span></span>
<span data-ttu-id="793a1-239">Запрос содержит недопустимый аргумент операции PATCH.</span><span class="sxs-lookup"><span data-stu-id="793a1-239">Your request contains an invalid PATCH argument. See Update page content.</span></span> <span data-ttu-id="793a1-240">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="793a1-240">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20122"></a><span data-ttu-id="793a1-241">20122</span><span class="sxs-lookup"><span data-stu-id="793a1-241">20122</span></span>
<span data-ttu-id="793a1-242">В запросе указано неподдерживаемое действие PATCH.</span><span class="sxs-lookup"><span data-stu-id="793a1-242">Your request specifies an unsupported PATCH action. See Update page content.</span></span> <span data-ttu-id="793a1-243">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="793a1-243">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20123"></a><span data-ttu-id="793a1-244">20123</span><span class="sxs-lookup"><span data-stu-id="793a1-244">20123</span></span>
<span data-ttu-id="793a1-245">PATCH-запросу не удается изменить указанную страницу.</span><span class="sxs-lookup"><span data-stu-id="793a1-245">The PATCH request is unable to alter the specified page.</span></span>

### <a name="20124"></a><span data-ttu-id="793a1-246">20124</span><span class="sxs-lookup"><span data-stu-id="793a1-246">20124</span></span>
<span data-ttu-id="793a1-247">Составной запрос PATCH не содержит раздела commands со структурой JSON действия PATCH.</span><span class="sxs-lookup"><span data-stu-id="793a1-247">Your multi-part PATCH request doesn’t include a 'commands' part with the PATCH action JSON structure. See Update page content.</span></span> <span data-ttu-id="793a1-248">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="793a1-248">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20125"></a><span data-ttu-id="793a1-249">20125</span><span class="sxs-lookup"><span data-stu-id="793a1-249">20125</span></span>
<span data-ttu-id="793a1-250">Запрос PATCH не содержит действий.</span><span class="sxs-lookup"><span data-stu-id="793a1-250">Your PATCH request contains no actions. See Update page content.</span></span> <span data-ttu-id="793a1-251">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="793a1-251">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20126"></a><span data-ttu-id="793a1-252">20126</span><span class="sxs-lookup"><span data-stu-id="793a1-252">20126</span></span>
<span data-ttu-id="793a1-253">Текст сообщения содержит неправильно отформатированный JSON или поля, неподдерживаемые для этой операции.</span><span class="sxs-lookup"><span data-stu-id="793a1-253">The message body contains either incorrectly formatted JSON or fields that are not supported for this operation.</span></span>

### <a name="20127"></a><span data-ttu-id="793a1-254">20127</span><span class="sxs-lookup"><span data-stu-id="793a1-254">20127</span></span>
<span data-ttu-id="793a1-255">Запрос указывает имя неизвестного свойства.</span><span class="sxs-lookup"><span data-stu-id="793a1-255">Your request specifies the name of an unknown property.</span></span>

### <a name="20128"></a><span data-ttu-id="793a1-256">20128</span><span class="sxs-lookup"><span data-stu-id="793a1-256">20128</span></span>
<span data-ttu-id="793a1-257">Запрос содержит ошибку синтаксиса OData в месте, указанном в сообщении.</span><span class="sxs-lookup"><span data-stu-id="793a1-257">Your request contains an OData syntax error at the position indicated in the message.</span></span>

### <a name="20129"></a><span data-ttu-id="793a1-258">20129</span><span class="sxs-lookup"><span data-stu-id="793a1-258">20129</span></span>
<span data-ttu-id="793a1-259">Запрос содержит параметр строки запроса **top** со слишком большим значением.</span><span class="sxs-lookup"><span data-stu-id="793a1-259">Your request contains a $top query whose value is too high.</span></span> <span data-ttu-id="793a1-260">Для запросов страниц максимальное значение составляет 100, а значение по умолчанию — 20.</span><span class="sxs-lookup"><span data-stu-id="793a1-260">For page queries, the maximum value is 100, and the default value is 20.</span></span>

### <a name="20130"></a><span data-ttu-id="793a1-261">20130</span><span class="sxs-lookup"><span data-stu-id="793a1-261">20130</span></span>
<span data-ttu-id="793a1-262">Запрос содержит URI, указывающий на HTTP-ресурс, который не удается найти.</span><span class="sxs-lookup"><span data-stu-id="793a1-262">Your request contains a URI that points to an HTTP resource that can’t be found.</span></span>

### <a name="20131"></a><span data-ttu-id="793a1-263">20131</span><span class="sxs-lookup"><span data-stu-id="793a1-263">20131</span></span>
<span data-ttu-id="793a1-264">Запрос содержит недопустимое значение Content-Type.</span><span class="sxs-lookup"><span data-stu-id="793a1-264">Your request contains an invalid data-tag attribute value.</span></span> <span data-ttu-id="793a1-265">Используйте значение, указанное в сообщении.</span><span class="sxs-lookup"><span data-stu-id="793a1-265">Use the value indicated in the message.</span></span> 

### <a name="20132"></a><span data-ttu-id="793a1-266">20132</span><span class="sxs-lookup"><span data-stu-id="793a1-266">20132</span></span>
<span data-ttu-id="793a1-267">Запрос содержит недопустимый контент.</span><span class="sxs-lookup"><span data-stu-id="793a1-267">Your request contains an invalid PATCH argument. See Update page content.</span></span> <span data-ttu-id="793a1-268">Распространенные причины этой проблемы — отсутствие заголовка запроса Content-Type и/или отсутствие содержимого в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="793a1-268">Your request contains invalid content. Common causes for this are a missing Content-Type request header and/or no content in the body of the request. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> 

### <a name="20133"></a><span data-ttu-id="793a1-269">20133</span><span class="sxs-lookup"><span data-stu-id="793a1-269">20133</span></span>
<span data-ttu-id="793a1-270">В запросе указан неподдерживаемый целевой объект операции PATCH.</span><span class="sxs-lookup"><span data-stu-id="793a1-270">Your request specifies a PATCH target that is not supported.  See Update page content.</span></span> <span data-ttu-id="793a1-271">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="793a1-271">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20134"></a><span data-ttu-id="793a1-272">20134</span><span class="sxs-lookup"><span data-stu-id="793a1-272">20134</span></span>
<span data-ttu-id="793a1-273">В запросе указан недопустимый элемент в качестве целевого объекта действия PATCH.</span><span class="sxs-lookup"><span data-stu-id="793a1-273">Your request specifies an invalid element as the target of the PATCH action.</span></span> <span data-ttu-id="793a1-274">Если в целевом объекте используется идентификатор **data-id**, убедитесь, что к нему добавлен префикс #.</span><span class="sxs-lookup"><span data-stu-id="793a1-274">Your request specifies an invalid element as the target of the PATCH action. If the target uses the **data-id** identifier, make sure it's prefixed with a # symbol. See Update page content.</span></span> <span data-ttu-id="793a1-275">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="793a1-275">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20135"></a><span data-ttu-id="793a1-276">20135</span><span class="sxs-lookup"><span data-stu-id="793a1-276">20135</span></span>
<span data-ttu-id="793a1-277">В запросе указан тип объекта, не поддерживаемый для операции PATCH.</span><span class="sxs-lookup"><span data-stu-id="793a1-277">Your request specifies an entity type that is not supported for the PATCH operation.</span></span> <span data-ttu-id="793a1-278">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="793a1-278">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20136"></a><span data-ttu-id="793a1-279">20136</span><span class="sxs-lookup"><span data-stu-id="793a1-279">20136</span></span>
<span data-ttu-id="793a1-280">Запрос содержит недопустимый атрибут **data-render-src** или **data-render-method**, либо этот атрибут отсутствует.</span><span class="sxs-lookup"><span data-stu-id="793a1-280">Your request contains an invalid or missing **data-render-src** or **data-render-method** attribute. See  Enrich captured content with the OneNote API.</span></span> <span data-ttu-id="793a1-281">См. статью [Извлечение данных из записей](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data).</span><span class="sxs-lookup"><span data-stu-id="793a1-281">See [Extract data from captures](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data).</span></span>

### <a name="20137"></a><span data-ttu-id="793a1-282">20137</span><span class="sxs-lookup"><span data-stu-id="793a1-282">20137</span></span>
<span data-ttu-id="793a1-283">Конечная страница не поддерживает PATCH-запросы.</span><span class="sxs-lookup"><span data-stu-id="793a1-283">The target page does not support PATCH requests.</span></span>

### <a name="20138"></a><span data-ttu-id="793a1-284">20138</span><span class="sxs-lookup"><span data-stu-id="793a1-284">20138</span></span>
<span data-ttu-id="793a1-285">Целевой тип элемента в запросе PATCH не поддерживает действие **append**.</span><span class="sxs-lookup"><span data-stu-id="793a1-285">The target element type in your PATCH request doesn't support the **append** action. See Update page content.</span></span> <span data-ttu-id="793a1-286">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="793a1-286">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20139"></a><span data-ttu-id="793a1-287">20139</span><span class="sxs-lookup"><span data-stu-id="793a1-287">20139</span></span>
<span data-ttu-id="793a1-288">Запрос содержит неподдерживаемое значение атрибута **data-tag**.</span><span class="sxs-lookup"><span data-stu-id="793a1-288">Your request contains an invalid **data-tag** attribute value.</span></span> <span data-ttu-id="793a1-289">См. статью [Использование тегов заметок](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags).</span><span class="sxs-lookup"><span data-stu-id="793a1-289">Use note tags</span></span>

### <a name="20140"></a><span data-ttu-id="793a1-290">20140</span><span class="sxs-lookup"><span data-stu-id="793a1-290">20140</span></span>
<span data-ttu-id="793a1-291">Запрос содержит недопустимое значение состояния **data-tag**.</span><span class="sxs-lookup"><span data-stu-id="793a1-291">Your request contains an invalid **data-tag** attribute value.</span></span> <span data-ttu-id="793a1-292">Теги заметок для флажков могут находиться в состоянии **completed**.</span><span class="sxs-lookup"><span data-stu-id="793a1-292">Check box note tags can have a **completed** status.</span></span> <span data-ttu-id="793a1-293">Пример.</span><span class="sxs-lookup"><span data-stu-id="793a1-293">Example:</span></span>
```html
    <p data-tag="to-do:completed">To-do note tag in completed state (checked box in the UI)</p>
```
<span data-ttu-id="793a1-294">См. статью [Использование тегов заметок](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags).</span><span class="sxs-lookup"><span data-stu-id="793a1-294">Use note tags</span></span>

### <a name="20141"></a><span data-ttu-id="793a1-295">20141</span><span class="sxs-lookup"><span data-stu-id="793a1-295">20141</span></span>
<span data-ttu-id="793a1-296">Целевой объект в запросе PATCH не поддерживает указанное действие.</span><span class="sxs-lookup"><span data-stu-id="793a1-296">The target in your PATCH request doesn't support the specified action.  See Update page content.</span></span> <span data-ttu-id="793a1-297">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="793a1-297">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20142"></a><span data-ttu-id="793a1-298">20142</span><span class="sxs-lookup"><span data-stu-id="793a1-298">20142</span></span>
<span data-ttu-id="793a1-299">Запрос содержит выражение **expand** для родительского объекта дочерних сущностей или дочернего объекта родительских сущностей. Такие выражения не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="793a1-299">Your request contains an **expand** expression for a parent of child entities or a child of parent entities, which  is not supported. See Supported OData query options.</span></span> <span data-ttu-id="793a1-300">См. раздел [Поддерживаемые параметры строки запроса OData](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-get-content#query-options).</span><span class="sxs-lookup"><span data-stu-id="793a1-300">Supported OData query string options</span></span>

### <a name="20143"></a><span data-ttu-id="793a1-301">20143</span><span class="sxs-lookup"><span data-stu-id="793a1-301">20143</span></span>
<span data-ttu-id="793a1-302">Недопустимый запрос OData.</span><span class="sxs-lookup"><span data-stu-id="793a1-302">The OData query is invalid.</span></span>

### <a name="20144"></a><span data-ttu-id="793a1-303">20144</span><span class="sxs-lookup"><span data-stu-id="793a1-303">20144</span></span>
<span data-ttu-id="793a1-304">Запрос содержит выражение **expand** для свойства, не связанного с навигацией.</span><span class="sxs-lookup"><span data-stu-id="793a1-304">Your request contains  an **expand** expression for a  non-navigation property. Only navigation properties can be expanded.</span></span> <span data-ttu-id="793a1-305">Расширять можно только свойства навигации.</span><span class="sxs-lookup"><span data-stu-id="793a1-305">Only navigation properties can be expanded.</span></span>

### <a name="20145"></a><span data-ttu-id="793a1-306">20145</span><span class="sxs-lookup"><span data-stu-id="793a1-306">20145</span></span>
<span data-ttu-id="793a1-307">Запрос содержит выражение **select** или **expand** с недопустимым термином.</span><span class="sxs-lookup"><span data-stu-id="793a1-307">The **select** or **expand** expression in your request contains an invalid term.</span></span>

### <a name="20146"></a><span data-ttu-id="793a1-308">20146</span><span class="sxs-lookup"><span data-stu-id="793a1-308">20146</span></span>
<span data-ttu-id="793a1-309">Для элемента указан атрибут `style="position:absolute"`, но в элементе **body** не указан атрибут `data-absolute-enabled="true"`, необходимый для поддержки позиционирования.</span><span class="sxs-lookup"><span data-stu-id="793a1-309">The **style="position:absolute"`style="position:absolute"` attribute is specified on an element, but  the body** element does not specify data-absolute-enabled="true"`data-absolute-enabled="true"`, which is required to support positioning.  All position settings are ignored.</span></span> <span data-ttu-id="793a1-310">Все параметры положения будут игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="793a1-310">All position settings will be ignored.</span></span> <span data-ttu-id="793a1-311">См. статью [Создание элементов с абсолютным положением](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span><span class="sxs-lookup"><span data-stu-id="793a1-311">See [Create absolute positioned elements](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span></span>

### <a name="20147"></a><span data-ttu-id="793a1-312">20147</span><span class="sxs-lookup"><span data-stu-id="793a1-312">20147</span></span>
<span data-ttu-id="793a1-313">Атрибут `style="position:absolute"` указан для элемента, не являющегося непосредственным дочерним объектом элемента **body**. Этот атрибут не поддерживается для таких элементов.</span><span class="sxs-lookup"><span data-stu-id="793a1-313">The `style="position:absolute"` attribute is specified on an element that is not a direct child of the **body** element, which is not supported.</span></span> <span data-ttu-id="793a1-314">Если это элемент **div**, **img** или **object**, сделайте его непосредственным дочерним объектом основного текста. В противном случае параметры положения будут проигнорированы, а содержимое будет отображаться внутри разделителя с абсолютным положением.</span><span class="sxs-lookup"><span data-stu-id="793a1-314">20147 The **style="position:absolute"** attribute is specified on an element that is not a direct child of the **body** element, which is not supported. If the element is a **div**, img, or object, make it a direct child of the body; otherwise the position settings will be ignored and its content will render inside an absolutely positioned div.</span></span> <span data-ttu-id="793a1-315">См. статью [Создание элементов с абсолютным положением](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span><span class="sxs-lookup"><span data-stu-id="793a1-315">See [Create absolute positioned elements](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span></span>

### <a name="20148"></a><span data-ttu-id="793a1-316">20148</span><span class="sxs-lookup"><span data-stu-id="793a1-316">20148</span></span>
<span data-ttu-id="793a1-317">Атрибут `style="position:absolute"` указан для элемента, тип которого не поддерживает этот атрибут.</span><span class="sxs-lookup"><span data-stu-id="793a1-317">20148  The  style="position:absolute"`style="position:absolute"` attribute is specified on an element type that does not  support it.  Only div, img, and object elements support positioning.</span></span> <span data-ttu-id="793a1-318">Позиционирование поддерживается только для элементов **div**, **img** и **object**, являющихся непосредственными дочерними элементами основного текста.</span><span class="sxs-lookup"><span data-stu-id="793a1-318">The  **style="position:absolute"** attribute is specified on an element type that does not  support it.  Only **div**, **img**, and object elements that are direct children of the page body support positioning.</span></span> <span data-ttu-id="793a1-319">См. статью [Создание элементов с абсолютным положением](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span><span class="sxs-lookup"><span data-stu-id="793a1-319">See [Create absolute positioned elements](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span></span>

### <a name="20149"></a><span data-ttu-id="793a1-320">20149</span><span class="sxs-lookup"><span data-stu-id="793a1-320">20149</span></span>
<span data-ttu-id="793a1-321">Запрос указывает целевой элемент, который не удается найти.</span><span class="sxs-lookup"><span data-stu-id="793a1-321">Your request specifies a target element that cannot be found.</span></span>

### <a name="20150"></a><span data-ttu-id="793a1-322">20150</span><span class="sxs-lookup"><span data-stu-id="793a1-322">20150</span></span>
<span data-ttu-id="793a1-323">Недопустимый запрос для этого типа проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="793a1-323">The request is not valid for this authentication type. Use the ../me/notes/ path  instead.</span></span> <span data-ttu-id="793a1-324">Используйте путь `../me/onenote/`.</span><span class="sxs-lookup"><span data-stu-id="793a1-324">Use the `../me/onenote/` path instead.</span></span>

### <a name="20151"></a><span data-ttu-id="793a1-325">20151</span><span class="sxs-lookup"><span data-stu-id="793a1-325">20151</span></span>
<span data-ttu-id="793a1-326">Недопустимый запрос для этого типа проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="793a1-326">The request is not valid for this authentication type. Use the ../me/notes/ path  instead.</span></span> <span data-ttu-id="793a1-327">Используйте конечную точку `../me/onenote/section/{id}/pages`, чтобы создать страницу в определенном разделе.</span><span class="sxs-lookup"><span data-stu-id="793a1-327">The request is not valid for this authentication type. Use the ../me/notes/section/{id}/pages`../me/onenote/section/{id}/pages` endpoint to create a page in a specific section.</span></span>

### <a name="20152"></a><span data-ttu-id="793a1-328">20152</span><span class="sxs-lookup"><span data-stu-id="793a1-328">20152 (EntityNameEmpty)</span></span>
<span data-ttu-id="793a1-329">Для объекта не указано значение имени.</span><span class="sxs-lookup"><span data-stu-id="793a1-329">There is no name value specified for the entity. The name must be defined, and it cannot contain whitespaces only.</span></span> <span data-ttu-id="793a1-330">Имя должно быть определено и не может содержать только пробелы.</span><span class="sxs-lookup"><span data-stu-id="793a1-330">There is no name value specified for the entity. The name must be defined, and it cannot contain whitespaces only.</span></span>

### <a name="20153"></a><span data-ttu-id="793a1-331">20153</span><span class="sxs-lookup"><span data-stu-id="793a1-331">20153 (EntityNameInvalidChar)</span></span>
<span data-ttu-id="793a1-332">Имя объекта содержит недопустимые символы.</span><span class="sxs-lookup"><span data-stu-id="793a1-332">The entity name contains invalid characters.</span></span> <span data-ttu-id="793a1-333">Имя не может содержать следующие символы: `? * \ / : < > | & # " % ~`</span><span class="sxs-lookup"><span data-stu-id="793a1-333">The entity name contains invalid characters. The name cannot contain the following characters: ?*\/:<>|&#''%~</span></span>

### <a name="20154"></a><span data-ttu-id="793a1-334">20154</span><span class="sxs-lookup"><span data-stu-id="793a1-334">20154 (EntityNameInvalidStart)</span></span>
<span data-ttu-id="793a1-335">Имя объекта не может начинаться с пробела.</span><span class="sxs-lookup"><span data-stu-id="793a1-335">The entity name cannot start with a space.</span></span>

### <a name="20155"></a><span data-ttu-id="793a1-336">20155</span><span class="sxs-lookup"><span data-stu-id="793a1-336">20155 (EntityNameTooLong)</span></span>
<span data-ttu-id="793a1-337">Слишком длинное имя объекта.</span><span class="sxs-lookup"><span data-stu-id="793a1-337">The name is too long.</span></span> <span data-ttu-id="793a1-338">Максимальная длина для имен записных книжек составляет 128 символов.</span><span class="sxs-lookup"><span data-stu-id="793a1-338">Notebook names have a 128-character limit.</span></span> <span data-ttu-id="793a1-339">Максимальная длина имен других объектов составляет 50 символов.</span><span class="sxs-lookup"><span data-stu-id="793a1-339">Other entity names have a 50-character limit.</span></span>

### <a name="20156"></a><span data-ttu-id="793a1-340">20156</span><span class="sxs-lookup"><span data-stu-id="793a1-340">20156</span></span>
<span data-ttu-id="793a1-341">Указанный идентификатор ресурса назначения не существует.</span><span class="sxs-lookup"><span data-stu-id="793a1-341">The specified ID for the destination resource does not exist.</span></span>

### <a name="20157"></a><span data-ttu-id="793a1-342">20157</span><span class="sxs-lookup"><span data-stu-id="793a1-342">20157</span></span>
<span data-ttu-id="793a1-343">Указан недопустимый идентификатор объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="793a1-343">The specified ID for the destination entity is invalid.</span></span>

### <a name="20158"></a><span data-ttu-id="793a1-344">20158</span><span class="sxs-lookup"><span data-stu-id="793a1-344">20158</span></span>
<span data-ttu-id="793a1-345">Не удалось получить метаданные для URL-адреса сайта, указанного в запросе.</span><span class="sxs-lookup"><span data-stu-id="793a1-345">Unable to get metadata for the site URL specified in the request.</span></span> <span data-ttu-id="793a1-346">Проверьте формат предоставленного URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="793a1-346">Check the format of the supplied URL.</span></span> <span data-ttu-id="793a1-347">К поддерживаемым форматам относятся `https://domain.sharepoint.com/site-a` и `https://domain.com/sites/site-a`.</span><span class="sxs-lookup"><span data-stu-id="793a1-347">Supported formats include `https://domain.sharepoint.com/site-a` and `https://domain.com/sites/site-a`.</span></span>

### <a name="20160"></a><span data-ttu-id="793a1-348">20160</span><span class="sxs-lookup"><span data-stu-id="793a1-348">20160</span></span>
<span data-ttu-id="793a1-349">Не удается найти единую группу Office 365 с указанным ИД.</span><span class="sxs-lookup"><span data-stu-id="793a1-349">Unable to find an Office 365 unified group that has the specified ID.</span></span>

### <a name="20161"></a><span data-ttu-id="793a1-350">20161</span><span class="sxs-lookup"><span data-stu-id="793a1-350">20161</span></span>
<span data-ttu-id="793a1-351">В контексте не указан действительный ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="793a1-351">The context does not specify a valid user ID.</span></span> <span data-ttu-id="793a1-352">Одна из распространенных ошибок — передача PUID/CID в виде значения типа long, а не hex.</span><span class="sxs-lookup"><span data-stu-id="793a1-352">The  context does not specify a valid user ID. One common error is that PUID/CID was passed in as a long instead of a hex.</span></span>

### <a name="20166"></a><span data-ttu-id="793a1-353">20166</span><span class="sxs-lookup"><span data-stu-id="793a1-353">20166</span></span>
<span data-ttu-id="793a1-354">Приложение отправило слишком много запросов от имени пользователя за короткий период времени.</span><span class="sxs-lookup"><span data-stu-id="793a1-354">The application has issued too many requests on behalf of a user in a short period of time.</span></span> <span data-ttu-id="793a1-355">Чтобы гарантировать стабильность и оперативность работы API OneNote, API возвращает код состояния 429 и это сообщение об ошибке, если обнаруживается, что приложение использует слишком много ресурсов.</span><span class="sxs-lookup"><span data-stu-id="793a1-355">To help ensure that the OneNote API remains stable and responsive, the API returns a 429 status code and this error when it detects that an application is using too many resources.</span></span> 

<span data-ttu-id="793a1-356">Дополнительные сведения см. в статье [Регулирование API OneNote и как его избежать](http://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx).</span><span class="sxs-lookup"><span data-stu-id="793a1-356">For more information, see [OneNote API throttling and how to avoid it](http://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx).</span></span>

### <a name="20168"></a><span data-ttu-id="793a1-357">20168</span><span class="sxs-lookup"><span data-stu-id="793a1-357">20168</span></span>
<span data-ttu-id="793a1-358">Источник видео, указанный в запросе, не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="793a1-358">The video source specified in the request is not supported.</span></span> <span data-ttu-id="793a1-359">См. актуальный список [поддерживаемых сайтов с видео](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#videos).</span><span class="sxs-lookup"><span data-stu-id="793a1-359">See [Supported video sites](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#videos) for the current list.</span></span>


## <a name="codes-from-30001-to-39999"></a><span data-ttu-id="793a1-360">Коды от 30001 до 39999</span><span class="sxs-lookup"><span data-stu-id="793a1-360">Codes from 30001 to 39999</span></span>
<span data-ttu-id="793a1-361">Что-то не так с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="793a1-361">Something is wrong with the user’s account.</span></span>

### <a name="30101"></a><span data-ttu-id="793a1-362">30101</span><span class="sxs-lookup"><span data-stu-id="793a1-362">30101</span></span>
<span data-ttu-id="793a1-363">Для учетной записи пользователя превышена квота OneDrive.</span><span class="sxs-lookup"><span data-stu-id="793a1-363">The user account has exceeded its OneDrive quota.</span></span> <span data-ttu-id="793a1-364">См. страницу [OneDrive](https://onedrive.live.com/about/en-us/).</span><span class="sxs-lookup"><span data-stu-id="793a1-364">See [OneDrive](https://onedrive.live.com/about/en-us/).</span></span>

### <a name="30102"></a><span data-ttu-id="793a1-365">30102</span><span class="sxs-lookup"><span data-stu-id="793a1-365">30102</span></span>
<span data-ttu-id="793a1-366">В запрошенные раздел невозможно что-либо добавить, так как он достиг своего максимального размера.</span><span class="sxs-lookup"><span data-stu-id="793a1-366">Nothing more can be added to the requested section because it has reached its maximum size.</span></span>

### <a name="30103"></a><span data-ttu-id="793a1-367">30103</span><span class="sxs-lookup"><span data-stu-id="793a1-367">30103</span></span>
<span data-ttu-id="793a1-368">Для выполнения запроса используется слишком много ресурсов.</span><span class="sxs-lookup"><span data-stu-id="793a1-368">Resource consumption is too high for the request.</span></span> <span data-ttu-id="793a1-369">Либо целевая учетная запись пользователя содержит слишком большой набор данных, либо служба получает слишком много одновременных запросов для одного сайта (например, личного сайта пользователя или сайта группы).</span><span class="sxs-lookup"><span data-stu-id="793a1-369">The level of resource consumption is too high. Either the target user account  has a large dataset or the service is receiving a high number of concurrent requests to the same site (for example, the user's personal site or a team site).</span></span>

### <a name="30104"></a><span data-ttu-id="793a1-370">30104</span><span class="sxs-lookup"><span data-stu-id="793a1-370">30104</span></span>
<span data-ttu-id="793a1-371">Работа учетной записи пользователя была приостановлена.</span><span class="sxs-lookup"><span data-stu-id="793a1-371">The user account has been suspended.</span></span>

### <a name="30105"></a><span data-ttu-id="793a1-372">30105</span><span class="sxs-lookup"><span data-stu-id="793a1-372">30105</span></span>
<span data-ttu-id="793a1-373">Личный сайт пользователя в OneDrive для бизнеса не подготовлен к работе. Это необходимо для доступа к записным книжкам.</span><span class="sxs-lookup"><span data-stu-id="793a1-373">The user's personal OneDrive for Business site is not provisioned, which is required to access notebooks.</span></span> <span data-ttu-id="793a1-374">Служба OneNote подготовит сайт к работе.</span><span class="sxs-lookup"><span data-stu-id="793a1-374">The OneNote service will provision the site now.</span></span> <span data-ttu-id="793a1-375">Этот процесс может занять несколько минут.</span><span class="sxs-lookup"><span data-stu-id="793a1-375">This process may take several minutes.</span></span>

### <a name="30106"></a><span data-ttu-id="793a1-376">30106</span><span class="sxs-lookup"><span data-stu-id="793a1-376">30106</span></span>
<span data-ttu-id="793a1-377">OneDrive для бизнеса подготавливается к работе для пользователя.</span><span class="sxs-lookup"><span data-stu-id="793a1-377">OneDrive for Business is being provisioned for the user.</span></span>

### <a name="30108"></a><span data-ttu-id="793a1-378">30108</span><span class="sxs-lookup"><span data-stu-id="793a1-378">30108</span></span>
<span data-ttu-id="793a1-379">Не удалось получить личное хранилище пользователя в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="793a1-379">The user's personal OneDrive for Business could not be retrieved.</span></span> <span data-ttu-id="793a1-380">В приведенной ниже таблице перечислены некоторые возможные причины.</span><span class="sxs-lookup"><span data-stu-id="793a1-380">The following table lists some possible causes.</span></span>

| <span data-ttu-id="793a1-381">Причина</span><span class="sxs-lookup"><span data-stu-id="793a1-381">Cause</span></span> | <span data-ttu-id="793a1-382">Решение</span><span class="sxs-lookup"><span data-stu-id="793a1-382">Resolution</span></span> |
|:------|:------|
| <span data-ttu-id="793a1-383">Личный сайт пользователя не подготовлен к работе.</span><span class="sxs-lookup"><span data-stu-id="793a1-383">The user's personal site has not been provisioned.</span></span> | <span data-ttu-id="793a1-384">Пользователь должен открыть OneDrive для бизнеса и следовать указаниям по подготовке сайта к работе.</span><span class="sxs-lookup"><span data-stu-id="793a1-384">The user should open OneDrive for Business and follow any instructions to provision the site.</span></span> <span data-ttu-id="793a1-385">Если проблема не будет устранена, необходимо обратиться к администратору клиента Office 365.</span><span class="sxs-lookup"><span data-stu-id="793a1-385">If this fails, they should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="793a1-386">В данный момент личный сайт пользователя подготавливается к работе.</span><span class="sxs-lookup"><span data-stu-id="793a1-386">The user's personal site is currently being provisioned.</span></span> | <span data-ttu-id="793a1-387">Попробуйте отправить запрос позже.</span><span class="sxs-lookup"><span data-stu-id="793a1-387">Try the request later.</span></span> |
| <span data-ttu-id="793a1-388">У пользователя нет действительной лицензии на OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="793a1-388">The user does not have a valid OneDrive for Business license.</span></span> | <span data-ttu-id="793a1-389">Пользователь должен обратиться к администратору своего клиента Office 365.</span><span class="sxs-lookup"><span data-stu-id="793a1-389">The user should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="793a1-390">Не удается отправить запрос из-за проблем с сетью.</span><span class="sxs-lookup"><span data-stu-id="793a1-390">A network issue prevented the request from being successfully sent.</span></span> | <span data-ttu-id="793a1-391">Попробуйте отправить запрос позже.</span><span class="sxs-lookup"><span data-stu-id="793a1-391">Try the request later.</span></span> |

### <a name="30109"></a><span data-ttu-id="793a1-392">30109</span><span class="sxs-lookup"><span data-stu-id="793a1-392">30109</span></span>
<span data-ttu-id="793a1-393">Некоторые пользователи, указанные в запросе, не существуют.</span><span class="sxs-lookup"><span data-stu-id="793a1-393">Some users in the request do not exist.</span></span>

### <a name="30110"></a><span data-ttu-id="793a1-394">30110</span><span class="sxs-lookup"><span data-stu-id="793a1-394">30110</span></span>
<span data-ttu-id="793a1-395">Для этого клиента не зарегистрированы службы сведений об учащихся.</span><span class="sxs-lookup"><span data-stu-id="793a1-395">Student Information Services has not been registered for this tenant.</span></span>

### <a name="30111"></a><span data-ttu-id="793a1-396">30111</span><span class="sxs-lookup"><span data-stu-id="793a1-396">30111</span></span>
<span data-ttu-id="793a1-397">Возникла общая ошибка служб сведений об учащихся.</span><span class="sxs-lookup"><span data-stu-id="793a1-397">There is a generic error with Student Information Services.</span></span>

### <a name="30112"></a><span data-ttu-id="793a1-398">30112</span><span class="sxs-lookup"><span data-stu-id="793a1-398">30112</span></span>
<span data-ttu-id="793a1-399">Запрос влияет на нескольких пользователей с одинаковыми именами.</span><span class="sxs-lookup"><span data-stu-id="793a1-399">Multiple users affected by the request had the same username.</span></span>

### <a name="30113"></a><span data-ttu-id="793a1-400">30113</span><span class="sxs-lookup"><span data-stu-id="793a1-400">30113</span></span>
<span data-ttu-id="793a1-401">Для записной книжки не разрешены приглашения.</span><span class="sxs-lookup"><span data-stu-id="793a1-401">The notebook is not configured to allow invites.</span></span>

### <a name="30114"></a><span data-ttu-id="793a1-402">30114</span><span class="sxs-lookup"><span data-stu-id="793a1-402">30114</span></span>
<span data-ttu-id="793a1-403">Отсутствует обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="793a1-403">There is a required parameter missing.</span></span>

## <a name="codes-from-40001-to-49999"></a><span data-ttu-id="793a1-404">Коды от 40001 до 49999</span><span class="sxs-lookup"><span data-stu-id="793a1-404">Codes from 40001 to 49999</span></span>
<span data-ttu-id="793a1-405">У пользователя или приложения нет необходимых разрешений.</span><span class="sxs-lookup"><span data-stu-id="793a1-405">The user or application does not have the correct permissions.</span></span>

### <a name="40001"></a><span data-ttu-id="793a1-406">40001</span><span class="sxs-lookup"><span data-stu-id="793a1-406">40001</span></span>
<span data-ttu-id="793a1-407">Запрос не содержит действительный маркер OAuth.</span><span class="sxs-lookup"><span data-stu-id="793a1-407">The request doesn’t contain a valid OAuth token. See  and  for more information.</span></span> <span data-ttu-id="793a1-408">См. раздел [Разрешения для заметок](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="793a1-408">See [Notes permissions](permissions_reference.md#notes-permissions).</span></span>

### <a name="40002"></a><span data-ttu-id="793a1-409">40002</span><span class="sxs-lookup"><span data-stu-id="793a1-409">40002</span></span>
<span data-ttu-id="793a1-410">У пользователя нет разрешения на запись в указанном расположении.</span><span class="sxs-lookup"><span data-stu-id="793a1-410">The user doesn’t have permission to write to the requested location.</span></span>

### <a name="40003"></a><span data-ttu-id="793a1-411">40003</span><span class="sxs-lookup"><span data-stu-id="793a1-411">40003</span></span>
<span data-ttu-id="793a1-412">У пользователя нет разрешения на доступ к запрашиваемому ресурсу.</span><span class="sxs-lookup"><span data-stu-id="793a1-412">The user doesn’t have permission to get access to the requested resource.</span></span>

### <a name="40004"></a><span data-ttu-id="793a1-413">40004</span><span class="sxs-lookup"><span data-stu-id="793a1-413">40004</span></span>
<span data-ttu-id="793a1-414">Область действия маркера OAuth недостаточна для выполнения запрашиваемого действия.</span><span class="sxs-lookup"><span data-stu-id="793a1-414">The OAuth token doesn’t have the required scopes to perform the requested action. See  for more information.</span></span> <span data-ttu-id="793a1-415">См. раздел [Разрешения для заметок](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="793a1-415">See [Notes permissions](permissions_reference.md#notes-permissions).</span></span>

### <a name="40006"></a><span data-ttu-id="793a1-416">40006</span><span class="sxs-lookup"><span data-stu-id="793a1-416">40006</span></span> 
<span data-ttu-id="793a1-417">Область действия маркера OAuth недостаточна для выполнения запрашиваемого действия.</span><span class="sxs-lookup"><span data-stu-id="793a1-417">The OAuth token doesn’t have the required scopes to perform the requested action. See  for more information.</span></span> <span data-ttu-id="793a1-418">В частности, это относится к разрешению на редактирование.</span><span class="sxs-lookup"><span data-stu-id="793a1-418">Specifically the edit permission.</span></span> <span data-ttu-id="793a1-419">См. раздел [Разрешения для заметок](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="793a1-419">See [Notes permissions](permissions_reference.md#notes-permissions).</span></span>

### <a name="40007"></a><span data-ttu-id="793a1-420">40007</span><span class="sxs-lookup"><span data-stu-id="793a1-420">40007</span></span>
<span data-ttu-id="793a1-421">У пользователя нет разрешений на доступ к этому ресурсу.</span><span class="sxs-lookup"><span data-stu-id="793a1-421">The user does not have permissions to access this resource.</span></span>

### <a name="40008"></a><span data-ttu-id="793a1-422">40008</span><span class="sxs-lookup"><span data-stu-id="793a1-422">40008</span></span>
<span data-ttu-id="793a1-423">Доступ к этому ресурсу запрещен.</span><span class="sxs-lookup"><span data-stu-id="793a1-423">Access is Forbidden for this resource.</span></span>

### <a name="40009"></a><span data-ttu-id="793a1-424">40009</span><span class="sxs-lookup"><span data-stu-id="793a1-424">40009</span></span>
<span data-ttu-id="793a1-425">Контейнер уже используется другим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="793a1-425">The container is already in use by another resource.</span></span>

## <a name="see-also"></a><span data-ttu-id="793a1-426">См. также</span><span class="sxs-lookup"><span data-stu-id="793a1-426">See also</span></span>

- [<span data-ttu-id="793a1-427">Сообщения об ошибках и типы ресурсов ошибок Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="793a1-427">Microsoft Graph error responses and resource types</span></span>](errors.md)
- [<span data-ttu-id="793a1-428">Справочник по OneNote</span><span class="sxs-lookup"><span data-stu-id="793a1-428">OneNote JavaScript API reference</span></span>](../api-reference/v1.0/resources/onenote.md)

