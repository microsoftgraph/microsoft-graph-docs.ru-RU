# <a name="error-codes-for-onenote-apis-in-microsoft-graph"></a><span data-ttu-id="56c6e-101">Коды ошибок для API OneNote в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="56c6e-101">Error codes for OneNote APIs in Microsoft Graph</span></span>

<span data-ttu-id="56c6e-102">В этой статье описываются коды ошибок, возвращаемые API OneNote в Microsoft Graph при сбоях запросов, отправляемых через API.</span><span class="sxs-lookup"><span data-stu-id="56c6e-102">This article describes error codes that are returned by the OneNote APIs in Microsoft Graph whenever a request sent through the API fails.</span></span>

## <a name="error-response-example"></a><span data-ttu-id="56c6e-103">Пример ответа об ошибке</span><span class="sxs-lookup"><span data-stu-id="56c6e-103">Error response example</span></span>
<span data-ttu-id="56c6e-104">Если при отправке запроса возникает ошибка, API OneNote перестает выполнять запрос и возвращает ответ об ошибке в виде объекта JSON.</span><span class="sxs-lookup"><span data-stu-id="56c6e-104">When your request generates an error, the OneNote API stops performing the request and returns an error response as a JSON object.</span></span> <span data-ttu-id="56c6e-105">Ответ об ошибке содержит соответствующий код ошибки, сообщение и ссылку на соответствующий раздел этой статьи.</span><span class="sxs-lookup"><span data-stu-id="56c6e-105">An error response contains the associated error code, a message, and a link to the appropriate section of this article.</span></span> <span data-ttu-id="56c6e-106">В приведенном ниже примере показано, как выглядит ответ об ошибке.</span><span class="sxs-lookup"><span data-stu-id="56c6e-106">The following example shows how an error response looks.</span></span>

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

<span data-ttu-id="56c6e-107">Дополнительные сведения об ошибках Microsoft Graph см. в статье [Сообщения об ошибках и типы ресурсов ошибок Microsoft Graph](errors.md).</span><span class="sxs-lookup"><span data-stu-id="56c6e-107">For more information about Microsoft Graph errors, see [Microsoft Graph error responses and resource types](errors.md).</span></span>

## <a name="codes-from-10001-to-19999"></a><span data-ttu-id="56c6e-108">Коды от 10001 до 19999</span><span class="sxs-lookup"><span data-stu-id="56c6e-108">Codes from 10001 to 19999</span></span>
<span data-ttu-id="56c6e-109">Служба работает с ошибками или отправляет информацию в приложение.</span><span class="sxs-lookup"><span data-stu-id="56c6e-109">The service is having problems or is sending information to the application.</span></span>

### <a name="10001"></a><span data-ttu-id="56c6e-110">10001</span><span class="sxs-lookup"><span data-stu-id="56c6e-110">10001</span></span>
<span data-ttu-id="56c6e-111">Произошла непредвиденная ошибка, и запрос не выполнен.</span><span class="sxs-lookup"><span data-stu-id="56c6e-111">An unexpected error occurred and the request failed.</span></span>

### <a name="10002"></a><span data-ttu-id="56c6e-112">10002</span><span class="sxs-lookup"><span data-stu-id="56c6e-112">10002</span></span>
<span data-ttu-id="56c6e-113">Служба в настоящее время недоступна.</span><span class="sxs-lookup"><span data-stu-id="56c6e-113">The service is not currently available.</span></span>

### <a name="10003"></a><span data-ttu-id="56c6e-114">10003</span><span class="sxs-lookup"><span data-stu-id="56c6e-114">10003</span></span>
<span data-ttu-id="56c6e-115">Учетная запись текущего пользователя превысила максимальное число активных запросов.</span><span class="sxs-lookup"><span data-stu-id="56c6e-115">The current user's account has exceeded the maximum number of active requests.</span></span> <span data-ttu-id="56c6e-116">Приложению придется повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="56c6e-116">Your app will have to repeat the request.</span></span>

### <a name="10004"></a><span data-ttu-id="56c6e-117">10004</span><span class="sxs-lookup"><span data-stu-id="56c6e-117">10004</span></span>
<span data-ttu-id="56c6e-118">Служба не может создать страницу в запрашиваемом разделе, так как раздел защищен паролем.</span><span class="sxs-lookup"><span data-stu-id="56c6e-118">The service can't create a page in the requested section because that section is protected by a password.</span></span>

### <a name="10005"></a><span data-ttu-id="56c6e-119">10005</span><span class="sxs-lookup"><span data-stu-id="56c6e-119">10005</span></span>
<span data-ttu-id="56c6e-120">В запросе превышено максимальное количество тегов изображений, в которых атрибут **data-render-src** содержит PDF-файл.</span><span class="sxs-lookup"><span data-stu-id="56c6e-120">The request contains more than the maximum number of image tags in which the **data-render-src** attribute contains a PDF.</span></span> <span data-ttu-id="56c6e-121">См. статью [Добавление изображений и файлов](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-images-files).</span><span class="sxs-lookup"><span data-stu-id="56c6e-121">See [Add images and files](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-images-files).</span></span>

### <a name="10006"></a><span data-ttu-id="56c6e-122">10006</span><span class="sxs-lookup"><span data-stu-id="56c6e-122">10006</span></span>
<span data-ttu-id="56c6e-123">API OneNote не удалось создать страницу в указанном разделе, потому что раздел поврежден.</span><span class="sxs-lookup"><span data-stu-id="56c6e-123">The OneNote API was unable to create a page in the specified section because that section is corrupt.</span></span>

### <a name="10007"></a><span data-ttu-id="56c6e-124">10007</span><span class="sxs-lookup"><span data-stu-id="56c6e-124">10007</span></span>
<span data-ttu-id="56c6e-p104">Сервер слишком занят, чтобы обработать входящий запрос в данный момент. Повторите попытку позже.</span><span class="sxs-lookup"><span data-stu-id="56c6e-p104">The server is too busy to handle the incoming request at this moment. Please try again later.</span></span>

### <a name="10008"></a><span data-ttu-id="56c6e-127">10008</span><span class="sxs-lookup"><span data-stu-id="56c6e-127">10008</span></span>
<span data-ttu-id="56c6e-128">Одна или несколько библиотек документов в хранилище OneDrive пользователя или группы содержит более 5000 элементов OneNote (записных книжек, разделов, групп разделов), и к ней невозможно отправлять запросы с помощью API.</span><span class="sxs-lookup"><span data-stu-id="56c6e-128">One or more of the document libraries on the user or group's OneDrive contains more than 5000 OneNote items (notebooks, sections, section groups), and cannot be queried using the API.</span></span> <span data-ttu-id="56c6e-129">Убедитесь, что ни одна из библиотек документов пользователей и групп не содержит более 5000 элементов OneNote.</span><span class="sxs-lookup"><span data-stu-id="56c6e-129">Please make sure that none of the user or group's document libraries contains more than 5000 OneNote items.</span></span> <span data-ttu-id="56c6e-130">Указания по устранению этой проблемы см. в [блоге разработчиков OneNote](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/).</span><span class="sxs-lookup"><span data-stu-id="56c6e-130">See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10012"></a><span data-ttu-id="56c6e-131">10012</span><span class="sxs-lookup"><span data-stu-id="56c6e-131">10012</span></span>
<span data-ttu-id="56c6e-132">Не удается создать или обновить объект, так как в библиотеке, содержащей записную книжку, требуется получать элементы для изменения, прежде чем редактировать их.</span><span class="sxs-lookup"><span data-stu-id="56c6e-132">Unable to create or update the entity because the library that contains the notebook requires items to be checked out before they can be edited.</span></span> <span data-ttu-id="56c6e-133">Дополнительные сведения см. в статье https://support.office.com/en-us/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7.</span><span class="sxs-lookup"><span data-stu-id="56c6e-133">For more information see https://support.office.com/en-us/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7</span></span>

<span data-ttu-id="56c6e-134">Отмените обязательное извлечение для этой библиотеки или переместите записную книжку.</span><span class="sxs-lookup"><span data-stu-id="56c6e-134">Either remove the check-out requirement from the library, or move the notebook.</span></span>

### <a name="10013"></a><span data-ttu-id="56c6e-135">10013</span><span class="sxs-lookup"><span data-stu-id="56c6e-135">10013</span></span>
<span data-ttu-id="56c6e-136">Одна или несколько библиотек документов в хранилище OneDrive пользователя или группы содержит более 20 000 элементов и не может быть индексирована для запросов с помощью API.</span><span class="sxs-lookup"><span data-stu-id="56c6e-136">One or more of the document libraries on the user or group's OneDrive contains more than 20,000 items and cannot be indexed for querying using the API.</span></span> <span data-ttu-id="56c6e-137">Убедитесь, что ни одна из библиотек документов пользователей и групп не содержит более 20 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="56c6e-137">Please make sure that none of the user or group's document libraries contains more than 20,000 items.</span></span> <span data-ttu-id="56c6e-138">Указания по устранению этой проблемы см. в [блоге разработчиков OneNote](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/).</span><span class="sxs-lookup"><span data-stu-id="56c6e-138">See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10014"></a><span data-ttu-id="56c6e-139">10014</span><span class="sxs-lookup"><span data-stu-id="56c6e-139">10014</span></span>
<span data-ttu-id="56c6e-140">В данный момент служба Azure Key Vault слишком занята для обработки входящего запроса.</span><span class="sxs-lookup"><span data-stu-id="56c6e-140">Azure Key Vault is too busy to handle the incoming request at this moment.</span></span> <span data-ttu-id="56c6e-141">Повторите попытку позже.</span><span class="sxs-lookup"><span data-stu-id="56c6e-141">Please try again later.</span></span>

### <a name="10015"></a><span data-ttu-id="56c6e-142">10015</span><span class="sxs-lookup"><span data-stu-id="56c6e-142">10015</span></span>
<span data-ttu-id="56c6e-143">В настоящее время среда SharePoint недоступна.</span><span class="sxs-lookup"><span data-stu-id="56c6e-143">SharePoint is currently unavailable.</span></span> <span data-ttu-id="56c6e-144">Повторите попытку позже.</span><span class="sxs-lookup"><span data-stu-id="56c6e-144">Please try again later.</span></span>

### <a name="10016"></a><span data-ttu-id="56c6e-145">10016</span><span class="sxs-lookup"><span data-stu-id="56c6e-145">10016</span></span>
<span data-ttu-id="56c6e-146">Библиотека документов в хранилище OneDrive пользователя или группы превысила пороговое количество уникальных областей безопасности.</span><span class="sxs-lookup"><span data-stu-id="56c6e-146">Document library on the user or group’s OneDrive exceeded unique security scopes threshold limit.</span></span> <span data-ttu-id="56c6e-147">Число уникальных областей безопасности для каждой библиотеки не может превышать 50 000.</span><span class="sxs-lookup"><span data-stu-id="56c6e-147">The maximum number of unique security scopes set for a library cannot exceed 50,000.</span></span>

### <a name="10017"></a><span data-ttu-id="56c6e-148">10017</span><span class="sxs-lookup"><span data-stu-id="56c6e-148">10017</span></span>
<span data-ttu-id="56c6e-149">Неправильный запрос.</span><span class="sxs-lookup"><span data-stu-id="56c6e-149">Bad Request.</span></span>

### <a name="19999"></a><span data-ttu-id="56c6e-150">19999</span><span class="sxs-lookup"><span data-stu-id="56c6e-150">19999</span></span>
<span data-ttu-id="56c6e-151">Запрос не выполнен из-за неизвестной ошибки.</span><span class="sxs-lookup"><span data-stu-id="56c6e-151">The request failed because an undetermined error occurred.</span></span>

## <a name="codes-from-20001-to-29999"></a><span data-ttu-id="56c6e-152">Коды от 20001 до 29999</span><span class="sxs-lookup"><span data-stu-id="56c6e-152">Codes from 20001 to 29999</span></span>
<span data-ttu-id="56c6e-153">Код приложения допустил ошибку.</span><span class="sxs-lookup"><span data-stu-id="56c6e-153">The application code has done something wrong.</span></span>

### <a name="20001"></a><span data-ttu-id="56c6e-154">20001</span><span class="sxs-lookup"><span data-stu-id="56c6e-154">20001</span></span>

<span data-ttu-id="56c6e-155">В запросе отсутствует необходимый раздел Presentation.</span><span class="sxs-lookup"><span data-stu-id="56c6e-155">The request is missing the required "Presentation" part.</span></span> <span data-ttu-id="56c6e-156">Он должен быть только один.</span><span class="sxs-lookup"><span data-stu-id="56c6e-156">Exactly one is required.</span></span> 

### <a name="20002"></a><span data-ttu-id="56c6e-157">20002</span><span class="sxs-lookup"><span data-stu-id="56c6e-157">20002</span></span>
<span data-ttu-id="56c6e-158">Запрос содержит две или более части Presentation.</span><span class="sxs-lookup"><span data-stu-id="56c6e-158">The request contains two or more "Presentation" parts.</span></span> <span data-ttu-id="56c6e-159">Он должен быть только один.</span><span class="sxs-lookup"><span data-stu-id="56c6e-159">Exactly one is required.</span></span>

### <a name="20003"></a><span data-ttu-id="56c6e-160">20003</span><span class="sxs-lookup"><span data-stu-id="56c6e-160">20003</span></span>
<span data-ttu-id="56c6e-161">В разделе Presentation допускаются только типы контента text/HTML и application/XHTML+XML.</span><span class="sxs-lookup"><span data-stu-id="56c6e-161">The content type of the "Presentation" part can be only text/HTML or application/XHTML+XML.</span></span> 

### <a name="20004"></a><span data-ttu-id="56c6e-162">20004</span><span class="sxs-lookup"><span data-stu-id="56c6e-162">20004</span></span>
<span data-ttu-id="56c6e-163">HTML-код раздела Presentation содержит тег image, в котором заданы свойства **src** и **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="56c6e-163">The "Presentation" part HTML contains an image tag with both the **src** and the **data-render-src** properties set.</span></span> <span data-ttu-id="56c6e-164">API проигнорирует свойство **src** и будет использовать свойство **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="56c6e-164">The API will ignore the **src** property and use the **data-render-src** property.</span></span> 

### <a name="20005"></a><span data-ttu-id="56c6e-165">20005</span><span class="sxs-lookup"><span data-stu-id="56c6e-165">20005</span></span>
<span data-ttu-id="56c6e-166">URI запроса слишком длинный.</span><span class="sxs-lookup"><span data-stu-id="56c6e-166">The request URI is too long.</span></span> <span data-ttu-id="56c6e-167">Максимальный размер URI (включая все параметры и данные) составляет 16 КБ или 16 384 символов.</span><span class="sxs-lookup"><span data-stu-id="56c6e-167">The maximum size of the URI (including all parameters and data) is 16 KB or 16,384 characters.</span></span>

### <a name="20006"></a><span data-ttu-id="56c6e-168">20006</span><span class="sxs-lookup"><span data-stu-id="56c6e-168">20006</span></span>
<span data-ttu-id="56c6e-169">HTML-код раздела Presentation содержит тег image, в котором не заданы свойства src и **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="56c6e-169">The "Presentation" part HTML contains an image tag with neither the src nor the **data-render-src** properties set.</span></span> <span data-ttu-id="56c6e-170">API проигнорирует тег **image**.</span><span class="sxs-lookup"><span data-stu-id="56c6e-170">The API will ignore the **image** tag.</span></span> 

### <a name="20007"></a><span data-ttu-id="56c6e-171">20007</span><span class="sxs-lookup"><span data-stu-id="56c6e-171">20007</span></span>
<span data-ttu-id="56c6e-172">HTML-код раздела Presentation содержит строку даты и времени создания, которая не соответствует ни одному из допустимых форматов.</span><span class="sxs-lookup"><span data-stu-id="56c6e-172">The "Presentation" part HTML contains a created date/time string that does not match any of the allowed formats.</span></span> 

### <a name="20008"></a><span data-ttu-id="56c6e-173">20008</span><span class="sxs-lookup"><span data-stu-id="56c6e-173">20008</span></span>
<span data-ttu-id="56c6e-174">Размер запроса превышает допустимый.</span><span class="sxs-lookup"><span data-stu-id="56c6e-174">The size of the request is too large.</span></span> 

### <a name="20009"></a><span data-ttu-id="56c6e-175">20009</span><span class="sxs-lookup"><span data-stu-id="56c6e-175">20009</span></span>
<span data-ttu-id="56c6e-176">Запрос содержит разделы с повторяющимися именами.</span><span class="sxs-lookup"><span data-stu-id="56c6e-176">The request contains parts with duplicate names.</span></span> <span data-ttu-id="56c6e-177">Имена разделов должны быть уникальными.</span><span class="sxs-lookup"><span data-stu-id="56c6e-177">Part names must be unique.</span></span> 

### <a name="20010"></a><span data-ttu-id="56c6e-178">20010</span><span class="sxs-lookup"><span data-stu-id="56c6e-178">20010</span></span>
<span data-ttu-id="56c6e-179">Для указанного типа контента не предоставлен заголовок Content-Disposition.</span><span class="sxs-lookup"><span data-stu-id="56c6e-179">The Content-Disposition header was not supplied for the specified content type.</span></span> 

### <a name="20011"></a><span data-ttu-id="56c6e-180">20011</span><span class="sxs-lookup"><span data-stu-id="56c6e-180">20011</span></span>
<span data-ttu-id="56c6e-181">Запрос содержит составные полезные данные неправильного формата.</span><span class="sxs-lookup"><span data-stu-id="56c6e-181">The request contains a malformed multipart payload.</span></span> <span data-ttu-id="56c6e-182">К возможным причинам этой ошибки относятся пустые строки, отсутствие последней строки, неправильно отформатированные разделители частей и т. д.</span><span class="sxs-lookup"><span data-stu-id="56c6e-182">Problems could include missing blank lines, a missing last line, incorrectly formatted part separators, and so on.</span></span> <span data-ttu-id="56c6e-183">Если вы создаете составное сообщение вручную, внимательно проверьте логику или используйте стороннюю библиотеку.</span><span class="sxs-lookup"><span data-stu-id="56c6e-183">If you're building the multipart message by hand, carefully check the logic, or consider using a third-party library.</span></span> 

### <a name="20012"></a><span data-ttu-id="56c6e-184">20012</span><span class="sxs-lookup"><span data-stu-id="56c6e-184">20012</span></span>
<span data-ttu-id="56c6e-185">В запросе не предоставлен тип контента для указанной части.</span><span class="sxs-lookup"><span data-stu-id="56c6e-185">The request doesn't supply a content type for the specified part.</span></span> 
### <a name="20013"></a><span data-ttu-id="56c6e-186">20013</span><span class="sxs-lookup"><span data-stu-id="56c6e-186">20013</span></span>
<span data-ttu-id="56c6e-187">В запросе не предоставлены заголовки Content-Type и Content-Disposition для указанной части.</span><span class="sxs-lookup"><span data-stu-id="56c6e-187">The request doesn't supply Content-Type and Content-Disposition headers for the specified part.</span></span> 

### <a name="20014"></a><span data-ttu-id="56c6e-188">20014</span><span class="sxs-lookup"><span data-stu-id="56c6e-188">20014</span></span>
<span data-ttu-id="56c6e-189">Длина части составного сообщения превышает максимальную (25 МБ).</span><span class="sxs-lookup"><span data-stu-id="56c6e-189">The length of a part in the multipart message exceeds the maximum size of 25 MB.</span></span> 

### <a name="20015"></a><span data-ttu-id="56c6e-190">20015</span><span class="sxs-lookup"><span data-stu-id="56c6e-190">20015</span></span>
<span data-ttu-id="56c6e-191">Количество частей составного сообщения превышает максимальное (500).</span><span class="sxs-lookup"><span data-stu-id="56c6e-191">The count of parts in the multipart message exceeds the limit of 500.</span></span> 

### <a name="20016"></a><span data-ttu-id="56c6e-192">20016</span><span class="sxs-lookup"><span data-stu-id="56c6e-192">20016</span></span>
<span data-ttu-id="56c6e-193">Длина составного сообщения превышает максимальную (75 МБ).</span><span class="sxs-lookup"><span data-stu-id="56c6e-193">The length of the multipart message exceeds the limit of 75 MB.</span></span> 

### <a name="20017"></a><span data-ttu-id="56c6e-194">20017</span><span class="sxs-lookup"><span data-stu-id="56c6e-194">20017</span></span>
<span data-ttu-id="56c6e-195">Неправильный формат MIME электронного сообщения.</span><span class="sxs-lookup"><span data-stu-id="56c6e-195">The email MIME was malformed.</span></span> 

### <a name="20018"></a><span data-ttu-id="56c6e-196">20018</span><span class="sxs-lookup"><span data-stu-id="56c6e-196">20018</span></span>
<span data-ttu-id="56c6e-197">Неправильный формат MIME или элемента ICal для собрания.</span><span class="sxs-lookup"><span data-stu-id="56c6e-197">The meeting MIME or ICal was malformed.</span></span> 

### <a name="20019"></a><span data-ttu-id="56c6e-198">20019</span><span class="sxs-lookup"><span data-stu-id="56c6e-198">20019</span></span>
<span data-ttu-id="56c6e-199">Элемент ICal не найден.</span><span class="sxs-lookup"><span data-stu-id="56c6e-199">No ICal was found.</span></span> 

### <a name="20020"></a><span data-ttu-id="56c6e-200">20020</span><span class="sxs-lookup"><span data-stu-id="56c6e-200">20020</span></span>
<span data-ttu-id="56c6e-201">В теле запроса обнаружен объект JSON неправильного формата.</span><span class="sxs-lookup"><span data-stu-id="56c6e-201">Encountered malformed Json in request body.</span></span> 

### <a name="20100"></a><span data-ttu-id="56c6e-202">20100</span><span class="sxs-lookup"><span data-stu-id="56c6e-202">20100</span></span>
<span data-ttu-id="56c6e-203">Ошибка синтаксиса запроса.</span><span class="sxs-lookup"><span data-stu-id="56c6e-203">Something is wrong with the syntax of your request.</span></span> 
### <a name="20101"></a><span data-ttu-id="56c6e-204">20101</span><span class="sxs-lookup"><span data-stu-id="56c6e-204">20101</span></span>
<span data-ttu-id="56c6e-205">Запрашиваемое свойство не существует.</span><span class="sxs-lookup"><span data-stu-id="56c6e-205">The property that you requested doesn't exist.</span></span>

### <a name="20102"></a><span data-ttu-id="56c6e-206">20102</span><span class="sxs-lookup"><span data-stu-id="56c6e-206">20102</span></span>
<span data-ttu-id="56c6e-207">Запрашиваемый ресурс не существует.</span><span class="sxs-lookup"><span data-stu-id="56c6e-207">You requested a resource that doesn't exist.</span></span>

### <a name="20103"></a><span data-ttu-id="56c6e-208">20103</span><span class="sxs-lookup"><span data-stu-id="56c6e-208">20103</span></span>
<span data-ttu-id="56c6e-209">Оператор **expand** не поддерживается для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="56c6e-209">The **expand** query is not supported for this request.</span></span> <span data-ttu-id="56c6e-210">См. раздел [Поддерживаемые параметры строки запроса OData](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-get-content#query-options).</span><span class="sxs-lookup"><span data-stu-id="56c6e-210">See [Supported OData query string options](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-get-content#query-options).</span></span>

### <a name="20104"></a><span data-ttu-id="56c6e-211">20104</span><span class="sxs-lookup"><span data-stu-id="56c6e-211">20104</span></span>
<span data-ttu-id="56c6e-212">Параметр запроса **pagelevel** поддерживается только для запросов к коллекции страниц в разделе или конкретной страницы.</span><span class="sxs-lookup"><span data-stu-id="56c6e-212">The **pagelevel** query option is supported only when querying for the pages collection in a section or for a specific page.</span></span> <span data-ttu-id="56c6e-213">Например:</span><span class="sxs-lookup"><span data-stu-id="56c6e-213">For example:</span></span>  

```http
GET ../sections/{id}/pages?pagelevel=true
GET ../pages/{id}?pagelevel=true
```

### <a name="20106"></a><span data-ttu-id="56c6e-214">20106</span><span class="sxs-lookup"><span data-stu-id="56c6e-214">20106</span></span>
<span data-ttu-id="56c6e-215">Запрос содержит неподдерживаемый оператор.</span><span class="sxs-lookup"><span data-stu-id="56c6e-215">Your request contains a query operator that is not supported.</span></span> 

### <a name="20108"></a><span data-ttu-id="56c6e-216">20108</span><span class="sxs-lookup"><span data-stu-id="56c6e-216">20108</span></span>
<span data-ttu-id="56c6e-217">Запрос содержит неподдерживаемые параметры запроса OData.</span><span class="sxs-lookup"><span data-stu-id="56c6e-217">Your request contains unsupported OData query parameters.</span></span>

### <a name="20109"></a><span data-ttu-id="56c6e-218">20109</span><span class="sxs-lookup"><span data-stu-id="56c6e-218">20109</span></span>
<span data-ttu-id="56c6e-219">Полезные данные в PATCH-запросе неправильно построены.</span><span class="sxs-lookup"><span data-stu-id="56c6e-219">The payload in the PATCH request is not constructed correctly.</span></span>

### <a name="20110"></a><span data-ttu-id="56c6e-220">20110</span><span class="sxs-lookup"><span data-stu-id="56c6e-220">20110</span></span>
<span data-ttu-id="56c6e-221">Для запросов на создание страниц с частями данных необходимо составное содержимое с разделом Presentation.</span><span class="sxs-lookup"><span data-stu-id="56c6e-221">Page create requests with data parts require the content to be multipart, with a "Presentation" part.</span></span> 

### <a name="20111"></a><span data-ttu-id="56c6e-222">20111</span><span class="sxs-lookup"><span data-stu-id="56c6e-222">20111</span></span>
<span data-ttu-id="56c6e-223">В запросе используется неподдерживаемая функция OData.</span><span class="sxs-lookup"><span data-stu-id="56c6e-223">Your request uses an OData feature that isn't supported.</span></span>

### <a name="20112"></a><span data-ttu-id="56c6e-224">20112</span><span class="sxs-lookup"><span data-stu-id="56c6e-224">20112</span></span>
<span data-ttu-id="56c6e-225">Запрос содержит недопустимый идентификатор для целевой сущности записной книжки, группы разделов, раздела или страницы.</span><span class="sxs-lookup"><span data-stu-id="56c6e-225">Your request contains an invalid ID for the target notebook, section group, section, or page entity.</span></span>

### <a name="20113"></a><span data-ttu-id="56c6e-226">20113</span><span class="sxs-lookup"><span data-stu-id="56c6e-226">20113</span></span>
<span data-ttu-id="56c6e-227">Ресурс, заданный в запросе, был удален.</span><span class="sxs-lookup"><span data-stu-id="56c6e-227">The resource specified in the request has been deleted.</span></span>

### <a name="20115"></a><span data-ttu-id="56c6e-228">20115</span><span class="sxs-lookup"><span data-stu-id="56c6e-228">20115</span></span>
<span data-ttu-id="56c6e-229">Имя содержит недопустимые символы.</span><span class="sxs-lookup"><span data-stu-id="56c6e-229">The name contains invalid characters.</span></span> <span data-ttu-id="56c6e-230">Имя записной книжки не может содержать следующие символы: `? * \ / : < > | ' "`</span><span class="sxs-lookup"><span data-stu-id="56c6e-230">A notebook name cannot contain any of the following characters: `? * \ / : < > | ' "`</span></span>

### <a name="20117"></a><span data-ttu-id="56c6e-231">20117</span><span class="sxs-lookup"><span data-stu-id="56c6e-231">20117</span></span>
<span data-ttu-id="56c6e-232">Элемент с таким именем уже существует в указанном месте.</span><span class="sxs-lookup"><span data-stu-id="56c6e-232">An item with the name you specified already exists in the location that you specified.</span></span>

### <a name="20119"></a><span data-ttu-id="56c6e-233">20119</span><span class="sxs-lookup"><span data-stu-id="56c6e-233">20119</span></span>
<span data-ttu-id="56c6e-234">HTML-код в разделе Presentation содержит атрибут **data-attachment**, который либо неправильно отформатирован либо содержит какие-либо из следующих недопустимых символов для имени файла: `\ / : * ? < > | "`.</span><span class="sxs-lookup"><span data-stu-id="56c6e-234">The HTML in the "Presentation" part contains a **data-attachment** attribute that either doesn't have a valid format or includes one or more of these invalid characters for a file name: `\ / : * ? < > | "`.</span></span> <span data-ttu-id="56c6e-235">Запрос заменил значение, указанное в сообщении об ошибке.</span><span class="sxs-lookup"><span data-stu-id="56c6e-235">The request substituted the value indicated in the error message.</span></span>

### <a name="20120"></a><span data-ttu-id="56c6e-236">20120</span><span class="sxs-lookup"><span data-stu-id="56c6e-236">20120</span></span>
<span data-ttu-id="56c6e-237">В запросе указан целевой объект операции PATCH, который не удается найти.</span><span class="sxs-lookup"><span data-stu-id="56c6e-237">Your request specifies a PATCH target that can't be located.</span></span>

### <a name="20121"></a><span data-ttu-id="56c6e-238">20121</span><span class="sxs-lookup"><span data-stu-id="56c6e-238">20121</span></span>
<span data-ttu-id="56c6e-239">Запрос содержит недопустимый аргумент операции PATCH.</span><span class="sxs-lookup"><span data-stu-id="56c6e-239">Your request contains an invalid PATCH argument.</span></span> <span data-ttu-id="56c6e-240">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="56c6e-240">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20122"></a><span data-ttu-id="56c6e-241">20122</span><span class="sxs-lookup"><span data-stu-id="56c6e-241">20122</span></span>
<span data-ttu-id="56c6e-242">В запросе указано неподдерживаемое действие PATCH.</span><span class="sxs-lookup"><span data-stu-id="56c6e-242">Your request specifies an unsupported PATCH action.</span></span> <span data-ttu-id="56c6e-243">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="56c6e-243">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20123"></a><span data-ttu-id="56c6e-244">20123</span><span class="sxs-lookup"><span data-stu-id="56c6e-244">20123</span></span>
<span data-ttu-id="56c6e-245">PATCH-запросу не удается изменить указанную страницу.</span><span class="sxs-lookup"><span data-stu-id="56c6e-245">The PATCH request is unable to alter the specified page.</span></span>

### <a name="20124"></a><span data-ttu-id="56c6e-246">20124</span><span class="sxs-lookup"><span data-stu-id="56c6e-246">20124</span></span>
<span data-ttu-id="56c6e-247">Составной запрос PATCH не содержит раздела commands со структурой JSON действия PATCH.</span><span class="sxs-lookup"><span data-stu-id="56c6e-247">Your multipart PATCH request doesn't include a "commands" part with the PATCH action JSON structure.</span></span> <span data-ttu-id="56c6e-248">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="56c6e-248">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20125"></a><span data-ttu-id="56c6e-249">20125</span><span class="sxs-lookup"><span data-stu-id="56c6e-249">20125</span></span>
<span data-ttu-id="56c6e-250">Запрос PATCH не содержит действий.</span><span class="sxs-lookup"><span data-stu-id="56c6e-250">Your PATCH request contains no actions.</span></span> <span data-ttu-id="56c6e-251">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="56c6e-251">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20126"></a><span data-ttu-id="56c6e-252">20126</span><span class="sxs-lookup"><span data-stu-id="56c6e-252">20126</span></span>
<span data-ttu-id="56c6e-253">Текст сообщения содержит неправильно отформатированный JSON или поля, неподдерживаемые для этой операции.</span><span class="sxs-lookup"><span data-stu-id="56c6e-253">The message body contains either incorrectly formatted JSON or fields that are not supported for this operation.</span></span>

### <a name="20127"></a><span data-ttu-id="56c6e-254">20127</span><span class="sxs-lookup"><span data-stu-id="56c6e-254">20127</span></span>
<span data-ttu-id="56c6e-255">Запрос указывает имя неизвестного свойства.</span><span class="sxs-lookup"><span data-stu-id="56c6e-255">Your request specifies the name of an unknown property.</span></span>

### <a name="20128"></a><span data-ttu-id="56c6e-256">20128</span><span class="sxs-lookup"><span data-stu-id="56c6e-256">20128</span></span>
<span data-ttu-id="56c6e-257">Запрос содержит ошибку синтаксиса OData в месте, указанном в сообщении.</span><span class="sxs-lookup"><span data-stu-id="56c6e-257">Your request contains an OData syntax error at the position indicated in the message.</span></span>

### <a name="20129"></a><span data-ttu-id="56c6e-258">20129</span><span class="sxs-lookup"><span data-stu-id="56c6e-258">20129</span></span>
<span data-ttu-id="56c6e-259">Запрос содержит параметр строки запроса **top** со слишком большим значением.</span><span class="sxs-lookup"><span data-stu-id="56c6e-259">Your request contains a **top** query string option whose value is too high.</span></span> <span data-ttu-id="56c6e-260">Для запросов страниц максимальное значение составляет 100, а значение по умолчанию — 20.</span><span class="sxs-lookup"><span data-stu-id="56c6e-260">For page queries, the maximum value is 100, and the default value is 20.</span></span>

### <a name="20130"></a><span data-ttu-id="56c6e-261">20130</span><span class="sxs-lookup"><span data-stu-id="56c6e-261">20130</span></span>
<span data-ttu-id="56c6e-262">Запрос содержит URI, указывающий на HTTP-ресурс, который не удается найти.</span><span class="sxs-lookup"><span data-stu-id="56c6e-262">Your request contains a URI that points to an HTTP resource that can't be found.</span></span>

### <a name="20131"></a><span data-ttu-id="56c6e-263">20131</span><span class="sxs-lookup"><span data-stu-id="56c6e-263">20131</span></span>
<span data-ttu-id="56c6e-264">Запрос содержит недопустимое значение Content-Type.</span><span class="sxs-lookup"><span data-stu-id="56c6e-264">Your request contains an invalid value for Content-Type.</span></span> <span data-ttu-id="56c6e-265">Используйте значение, указанное в сообщении.</span><span class="sxs-lookup"><span data-stu-id="56c6e-265">Use the value indicated in the message.</span></span> 

### <a name="20132"></a><span data-ttu-id="56c6e-266">20132</span><span class="sxs-lookup"><span data-stu-id="56c6e-266">20132</span></span>
<span data-ttu-id="56c6e-267">Запрос содержит недопустимый контент.</span><span class="sxs-lookup"><span data-stu-id="56c6e-267">Your request contains invalid content.</span></span> <span data-ttu-id="56c6e-268">Распространенные причины этой проблемы — отсутствие заголовка запроса Content-Type и/или отсутствие содержимого в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="56c6e-268">Common causes for this are a missing Content-Type request header and/or no content in the body of the request.</span></span> 

### <a name="20133"></a><span data-ttu-id="56c6e-269">20133</span><span class="sxs-lookup"><span data-stu-id="56c6e-269">20133</span></span>
<span data-ttu-id="56c6e-270">В запросе указан неподдерживаемый целевой объект операции PATCH.</span><span class="sxs-lookup"><span data-stu-id="56c6e-270">Your request specifies a PATCH target that is not supported.</span></span> <span data-ttu-id="56c6e-271">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="56c6e-271">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20134"></a><span data-ttu-id="56c6e-272">20134</span><span class="sxs-lookup"><span data-stu-id="56c6e-272">20134</span></span>
<span data-ttu-id="56c6e-273">В запросе указан недопустимый элемент в качестве целевого объекта действия PATCH.</span><span class="sxs-lookup"><span data-stu-id="56c6e-273">Your request specifies an invalid element as the target of the PATCH action.</span></span> <span data-ttu-id="56c6e-274">Если в целевом объекте используется идентификатор **data-id**, убедитесь, что к нему добавлен префикс #.</span><span class="sxs-lookup"><span data-stu-id="56c6e-274">If the target uses the **data-id** identifier, make sure it's prefixed with a # symbol.</span></span> <span data-ttu-id="56c6e-275">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="56c6e-275">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20135"></a><span data-ttu-id="56c6e-276">20135</span><span class="sxs-lookup"><span data-stu-id="56c6e-276">20135</span></span>
<span data-ttu-id="56c6e-277">В запросе указан тип объекта, не поддерживаемый для операции PATCH.</span><span class="sxs-lookup"><span data-stu-id="56c6e-277">Your request specifies an entity type that is not supported for the PATCH operation.</span></span> <span data-ttu-id="56c6e-278">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="56c6e-278">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20136"></a><span data-ttu-id="56c6e-279">20136</span><span class="sxs-lookup"><span data-stu-id="56c6e-279">20136</span></span>
<span data-ttu-id="56c6e-280">Запрос содержит недопустимый атрибут **data-render-src** или **data-render-method**, либо этот атрибут отсутствует.</span><span class="sxs-lookup"><span data-stu-id="56c6e-280">Your request contains an invalid or missing **data-render-src** or **data-render-method** attribute.</span></span> <span data-ttu-id="56c6e-281">См. статью [Извлечение данных из записей](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-extract-data).</span><span class="sxs-lookup"><span data-stu-id="56c6e-281">See [Extract data from captures](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-extract-data).</span></span>

### <a name="20137"></a><span data-ttu-id="56c6e-282">20137</span><span class="sxs-lookup"><span data-stu-id="56c6e-282">20137</span></span>
<span data-ttu-id="56c6e-283">Конечная страница не поддерживает PATCH-запросы.</span><span class="sxs-lookup"><span data-stu-id="56c6e-283">The target page does not support PATCH requests.</span></span>

### <a name="20138"></a><span data-ttu-id="56c6e-284">20138</span><span class="sxs-lookup"><span data-stu-id="56c6e-284">20138</span></span>
<span data-ttu-id="56c6e-285">Целевой тип элемента в запросе PATCH не поддерживает действие **append**.</span><span class="sxs-lookup"><span data-stu-id="56c6e-285">The target element type in your PATCH request doesn't support the **append** action.</span></span> <span data-ttu-id="56c6e-286">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="56c6e-286">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20139"></a><span data-ttu-id="56c6e-287">20139</span><span class="sxs-lookup"><span data-stu-id="56c6e-287">20139</span></span>
<span data-ttu-id="56c6e-288">Запрос содержит неподдерживаемое значение атрибута **data-tag**.</span><span class="sxs-lookup"><span data-stu-id="56c6e-288">Your request contains an invalid **data-tag** attribute value.</span></span> <span data-ttu-id="56c6e-289">См. статью [Использование тегов заметок](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-note-tags).</span><span class="sxs-lookup"><span data-stu-id="56c6e-289">See [Use note tags](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-note-tags).</span></span>

### <a name="20140"></a><span data-ttu-id="56c6e-290">20140</span><span class="sxs-lookup"><span data-stu-id="56c6e-290">20140</span></span>
<span data-ttu-id="56c6e-291">Запрос содержит недопустимое значение состояния **data-tag**.</span><span class="sxs-lookup"><span data-stu-id="56c6e-291">Your request contains an invalid **data-tag** status value.</span></span> <span data-ttu-id="56c6e-292">Теги заметок для флажков могут находиться в состоянии **completed**.</span><span class="sxs-lookup"><span data-stu-id="56c6e-292">Check box note tags can have a **completed** status.</span></span> <span data-ttu-id="56c6e-293">Пример.</span><span class="sxs-lookup"><span data-stu-id="56c6e-293">Example:</span></span>
```html
    <p data-tag="to-do:completed">To-do note tag in completed state (checked box in the UI)</p>
```
<span data-ttu-id="56c6e-294">См. статью [Использование тегов заметок](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-note-tags).</span><span class="sxs-lookup"><span data-stu-id="56c6e-294">See [Use note tags](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-note-tags).</span></span>

### <a name="20141"></a><span data-ttu-id="56c6e-295">20141</span><span class="sxs-lookup"><span data-stu-id="56c6e-295">20141</span></span>
<span data-ttu-id="56c6e-296">Целевой объект в запросе PATCH не поддерживает указанное действие.</span><span class="sxs-lookup"><span data-stu-id="56c6e-296">The target in your PATCH request doesn't support the specified action.</span></span> <span data-ttu-id="56c6e-297">См. статью [Обновление содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="56c6e-297">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20142"></a><span data-ttu-id="56c6e-298">20142</span><span class="sxs-lookup"><span data-stu-id="56c6e-298">20142</span></span>
<span data-ttu-id="56c6e-299">Запрос содержит выражение **expand** для родительского объекта дочерних сущностей или дочернего объекта родительских сущностей. Такие выражения не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="56c6e-299">Your request contains an **expand** expression for a parent of child entities or a child of parent entities, which is not supported.</span></span> <span data-ttu-id="56c6e-300">См. раздел [Поддерживаемые параметры строки запроса OData](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-get-content#query-options).</span><span class="sxs-lookup"><span data-stu-id="56c6e-300">See [Supported OData query string options](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-get-content#query-options).</span></span>

### <a name="20143"></a><span data-ttu-id="56c6e-301">20143</span><span class="sxs-lookup"><span data-stu-id="56c6e-301">20143</span></span>
<span data-ttu-id="56c6e-302">Недопустимый запрос OData.</span><span class="sxs-lookup"><span data-stu-id="56c6e-302">The OData query is invalid.</span></span>

### <a name="20144"></a><span data-ttu-id="56c6e-303">20144</span><span class="sxs-lookup"><span data-stu-id="56c6e-303">20144</span></span>
<span data-ttu-id="56c6e-304">Запрос содержит выражение **expand** для свойства, не связанного с навигацией.</span><span class="sxs-lookup"><span data-stu-id="56c6e-304">Your request contains an **expand** expression for a non-navigation property.</span></span> <span data-ttu-id="56c6e-305">Расширять можно только свойства навигации.</span><span class="sxs-lookup"><span data-stu-id="56c6e-305">Only navigation properties can be expanded.</span></span>

### <a name="20145"></a><span data-ttu-id="56c6e-306">20145</span><span class="sxs-lookup"><span data-stu-id="56c6e-306">20145</span></span>
<span data-ttu-id="56c6e-307">Запрос содержит выражение **select** или **expand** с недопустимым термином.</span><span class="sxs-lookup"><span data-stu-id="56c6e-307">The **select** or **expand** expression in your request contains an invalid term.</span></span>

### <a name="20146"></a><span data-ttu-id="56c6e-308">20146</span><span class="sxs-lookup"><span data-stu-id="56c6e-308">20146</span></span>
<span data-ttu-id="56c6e-309">Для элемента указан атрибут `style="position:absolute"`, но в элементе **body** не указан атрибут `data-absolute-enabled="true"`, необходимый для поддержки позиционирования.</span><span class="sxs-lookup"><span data-stu-id="56c6e-309">The `style="position:absolute"` attribute is specified on an element, but the **body** element does not specify `data-absolute-enabled="true"`, which is required to support positioning.</span></span> <span data-ttu-id="56c6e-310">Все параметры положения будут игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="56c6e-310">All position settings will be ignored.</span></span> <span data-ttu-id="56c6e-311">См. статью [Создание элементов с абсолютным положением](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="56c6e-311">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20147"></a><span data-ttu-id="56c6e-312">20147</span><span class="sxs-lookup"><span data-stu-id="56c6e-312">20147</span></span>
<span data-ttu-id="56c6e-313">Атрибут `style="position:absolute"` указан для элемента, не являющегося непосредственным дочерним объектом элемента **body**. Этот атрибут не поддерживается для таких элементов.</span><span class="sxs-lookup"><span data-stu-id="56c6e-313">The `style="position:absolute"` attribute is specified on an element that is not a direct child of the **body** element, which is not supported.</span></span> <span data-ttu-id="56c6e-314">Если это элемент **div**, **img** или **object**, сделайте его непосредственным дочерним объектом основного текста. В противном случае параметры положения будут проигнорированы, а содержимое будет отображаться внутри разделителя с абсолютным положением.</span><span class="sxs-lookup"><span data-stu-id="56c6e-314">If the element is a **div**, **img**, or **object**, make it a direct child of the body; otherwise the position settings will be ignored and its content will render inside an absolute positioned div.</span></span> <span data-ttu-id="56c6e-315">См. статью [Создание элементов с абсолютным положением](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="56c6e-315">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20148"></a><span data-ttu-id="56c6e-316">20148</span><span class="sxs-lookup"><span data-stu-id="56c6e-316">20148</span></span>
<span data-ttu-id="56c6e-317">Атрибут `style="position:absolute"` указан для элемента, тип которого не поддерживает этот атрибут.</span><span class="sxs-lookup"><span data-stu-id="56c6e-317">The `style="position:absolute"` attribute is specified on an element type that does not support it.</span></span> <span data-ttu-id="56c6e-318">Позиционирование поддерживается только для элементов **div**, **img** и **object**, являющихся непосредственными дочерними элементами основного текста.</span><span class="sxs-lookup"><span data-stu-id="56c6e-318">Only **div**, **img**, and **object** elements that are direct children of the page body support positioning.</span></span> <span data-ttu-id="56c6e-319">См. статью [Создание элементов с абсолютным положением](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="56c6e-319">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20149"></a><span data-ttu-id="56c6e-320">20149</span><span class="sxs-lookup"><span data-stu-id="56c6e-320">20149</span></span>
<span data-ttu-id="56c6e-321">Запрос указывает целевой элемент, который не удается найти.</span><span class="sxs-lookup"><span data-stu-id="56c6e-321">Your request specifies a target element that cannot be found.</span></span>

### <a name="20150"></a><span data-ttu-id="56c6e-322">20150</span><span class="sxs-lookup"><span data-stu-id="56c6e-322">20150</span></span>
<span data-ttu-id="56c6e-323">Недопустимый запрос для этого типа проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="56c6e-323">The request is not valid for this authentication type.</span></span> <span data-ttu-id="56c6e-324">Используйте путь `../me/onenote/`.</span><span class="sxs-lookup"><span data-stu-id="56c6e-324">Use the `../me/onenote/` path instead.</span></span>

### <a name="20151"></a><span data-ttu-id="56c6e-325">20151</span><span class="sxs-lookup"><span data-stu-id="56c6e-325">20151</span></span>
<span data-ttu-id="56c6e-326">Недопустимый запрос для этого типа проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="56c6e-326">The request is not valid for this authentication type.</span></span> <span data-ttu-id="56c6e-327">Используйте конечную точку `../me/onenote/section/{id}/pages`, чтобы создать страницу в определенном разделе.</span><span class="sxs-lookup"><span data-stu-id="56c6e-327">Use the `../me/onenote/section/{id}/pages` endpoint to create a page in a specific section.</span></span>

### <a name="20152"></a><span data-ttu-id="56c6e-328">20152</span><span class="sxs-lookup"><span data-stu-id="56c6e-328">20152</span></span>
<span data-ttu-id="56c6e-329">Для объекта не указано значение имени.</span><span class="sxs-lookup"><span data-stu-id="56c6e-329">There is no name value specified for the entity.</span></span> <span data-ttu-id="56c6e-330">Имя должно быть определено и не может содержать только пробелы.</span><span class="sxs-lookup"><span data-stu-id="56c6e-330">The name must be defined, and it cannot contain whitespaces only.</span></span>

### <a name="20153"></a><span data-ttu-id="56c6e-331">20153</span><span class="sxs-lookup"><span data-stu-id="56c6e-331">20153</span></span>
<span data-ttu-id="56c6e-332">Имя объекта содержит недопустимые символы.</span><span class="sxs-lookup"><span data-stu-id="56c6e-332">The entity name contains invalid characters.</span></span> <span data-ttu-id="56c6e-333">Имя не может содержать следующие символы: `? * \ / : < > | & # " % ~`</span><span class="sxs-lookup"><span data-stu-id="56c6e-333">The name cannot contain the following characters: `? * \ / : < > | & # " % ~`</span></span>

### <a name="20154"></a><span data-ttu-id="56c6e-334">20154</span><span class="sxs-lookup"><span data-stu-id="56c6e-334">20154</span></span>
<span data-ttu-id="56c6e-335">Имя объекта не может начинаться с пробела.</span><span class="sxs-lookup"><span data-stu-id="56c6e-335">The entity name cannot start with a space.</span></span>

### <a name="20155"></a><span data-ttu-id="56c6e-336">20155</span><span class="sxs-lookup"><span data-stu-id="56c6e-336">20155</span></span>
<span data-ttu-id="56c6e-337">Слишком длинное имя объекта.</span><span class="sxs-lookup"><span data-stu-id="56c6e-337">The entity name is too long.</span></span> <span data-ttu-id="56c6e-338">Максимальная длина для имен записных книжек составляет 128 символов.</span><span class="sxs-lookup"><span data-stu-id="56c6e-338">Notebook names have a 128-character limit.</span></span> <span data-ttu-id="56c6e-339">Максимальная длина имен других объектов составляет 50 символов.</span><span class="sxs-lookup"><span data-stu-id="56c6e-339">Other entity names have a 50-character limit.</span></span>

### <a name="20156"></a><span data-ttu-id="56c6e-340">20156</span><span class="sxs-lookup"><span data-stu-id="56c6e-340">20156</span></span>
<span data-ttu-id="56c6e-341">Указанный идентификатор ресурса назначения не существует.</span><span class="sxs-lookup"><span data-stu-id="56c6e-341">The specified ID for the destination resource does not exist.</span></span>

### <a name="20157"></a><span data-ttu-id="56c6e-342">20157</span><span class="sxs-lookup"><span data-stu-id="56c6e-342">20157</span></span>
<span data-ttu-id="56c6e-343">Указан недопустимый идентификатор объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="56c6e-343">The specified ID for the destination entity is invalid.</span></span>

### <a name="20158"></a><span data-ttu-id="56c6e-344">20158</span><span class="sxs-lookup"><span data-stu-id="56c6e-344">20158</span></span>
<span data-ttu-id="56c6e-345">Не удалось получить метаданные для URL-адреса сайта, указанного в запросе.</span><span class="sxs-lookup"><span data-stu-id="56c6e-345">Unable to get metadata for the site URL specified in the request.</span></span> <span data-ttu-id="56c6e-346">Проверьте формат предоставленного URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="56c6e-346">Check the format of the supplied URL.</span></span> <span data-ttu-id="56c6e-347">К поддерживаемым форматам относятся `https://domain.sharepoint.com/site-a` и `https://domain.com/sites/site-a`.</span><span class="sxs-lookup"><span data-stu-id="56c6e-347">Supported formats include `https://domain.sharepoint.com/site-a` and `https://domain.com/sites/site-a`.</span></span>

### <a name="20160"></a><span data-ttu-id="56c6e-348">20160</span><span class="sxs-lookup"><span data-stu-id="56c6e-348">20160</span></span>
<span data-ttu-id="56c6e-349">Не удается найти единую группу Office 365 с указанным ИД.</span><span class="sxs-lookup"><span data-stu-id="56c6e-349">Unable to find an Office 365 unified group that has the specified ID.</span></span>

### <a name="20161"></a><span data-ttu-id="56c6e-350">20161</span><span class="sxs-lookup"><span data-stu-id="56c6e-350">20161</span></span>
<span data-ttu-id="56c6e-351">В контексте не указан действительный ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="56c6e-351">The context does not specify a valid user ID.</span></span> <span data-ttu-id="56c6e-352">Одна из распространенных ошибок — передача PUID/CID в виде значения типа long, а не hex.</span><span class="sxs-lookup"><span data-stu-id="56c6e-352">One common error is that PUID/CID was passed in as a long instead of a hex.</span></span>

### <a name="20166"></a><span data-ttu-id="56c6e-353">20166</span><span class="sxs-lookup"><span data-stu-id="56c6e-353">20166</span></span>
<span data-ttu-id="56c6e-354">Приложение отправило слишком много запросов от имени пользователя за короткий период времени.</span><span class="sxs-lookup"><span data-stu-id="56c6e-354">The application has issued too many requests on behalf of a user in a short period of time.</span></span> <span data-ttu-id="56c6e-355">Чтобы гарантировать стабильность и оперативность работы API OneNote, API возвращает код состояния 429 и это сообщение об ошибке, если обнаруживается, что приложение использует слишком много ресурсов.</span><span class="sxs-lookup"><span data-stu-id="56c6e-355">To help ensure that the OneNote API remains stable and responsive, the API returns a 429 status code and this error when it detects that an application is using too many resources.</span></span> 

<span data-ttu-id="56c6e-356">Дополнительные сведения см. в статье [Регулирование API OneNote и как его избежать](http://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx).</span><span class="sxs-lookup"><span data-stu-id="56c6e-356">For more information, see [OneNote API throttling and how to avoid it](http://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx).</span></span>

### <a name="20168"></a><span data-ttu-id="56c6e-357">20168</span><span class="sxs-lookup"><span data-stu-id="56c6e-357">20168</span></span>
<span data-ttu-id="56c6e-358">Источник видео, указанный в запросе, не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56c6e-358">The video source specified in the request is not supported.</span></span> <span data-ttu-id="56c6e-359">См. актуальный список [поддерживаемых сайтов с видео](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-images-files#videos).</span><span class="sxs-lookup"><span data-stu-id="56c6e-359">See [Supported video sites](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-images-files#videos) for the current list.</span></span>


## <a name="codes-from-30001-to-39999"></a><span data-ttu-id="56c6e-360">Коды от 30001 до 39999</span><span class="sxs-lookup"><span data-stu-id="56c6e-360">Codes from 30001 to 39999</span></span>
<span data-ttu-id="56c6e-361">Что-то не так с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="56c6e-361">Something is wrong with the user's account.</span></span>

### <a name="30101"></a><span data-ttu-id="56c6e-362">30101</span><span class="sxs-lookup"><span data-stu-id="56c6e-362">30101</span></span>
<span data-ttu-id="56c6e-363">Для учетной записи пользователя превышена квота OneDrive.</span><span class="sxs-lookup"><span data-stu-id="56c6e-363">The user account has exceeded its OneDrive quota.</span></span> <span data-ttu-id="56c6e-364">См. страницу [OneDrive](https://onedrive.live.com/about/ru-RU/).</span><span class="sxs-lookup"><span data-stu-id="56c6e-364">See [OneDrive](https://onedrive.live.com/about/ru-RU/).</span></span>

### <a name="30102"></a><span data-ttu-id="56c6e-365">30102</span><span class="sxs-lookup"><span data-stu-id="56c6e-365">30102</span></span>
<span data-ttu-id="56c6e-366">В запрошенные раздел невозможно что-либо добавить, так как он достиг своего максимального размера.</span><span class="sxs-lookup"><span data-stu-id="56c6e-366">Nothing more can be added to the requested section because it has reached its maximum size.</span></span>

### <a name="30103"></a><span data-ttu-id="56c6e-367">30103</span><span class="sxs-lookup"><span data-stu-id="56c6e-367">30103</span></span>
<span data-ttu-id="56c6e-368">Для выполнения запроса используется слишком много ресурсов.</span><span class="sxs-lookup"><span data-stu-id="56c6e-368">Resource consumption is too high for the request.</span></span> <span data-ttu-id="56c6e-369">Либо целевая учетная запись пользователя содержит слишком большой набор данных, либо служба получает слишком много одновременных запросов для одного сайта (например, личного сайта пользователя или сайта группы).</span><span class="sxs-lookup"><span data-stu-id="56c6e-369">Either the target user account has a large dataset, or the service is receiving a high number of concurrent requests to the same site (for example, the user's personal site or a team site).</span></span>

### <a name="30104"></a><span data-ttu-id="56c6e-370">30104</span><span class="sxs-lookup"><span data-stu-id="56c6e-370">30104</span></span>
<span data-ttu-id="56c6e-371">Работа учетной записи пользователя была приостановлена.</span><span class="sxs-lookup"><span data-stu-id="56c6e-371">The user account has been suspended.</span></span>

### <a name="30105"></a><span data-ttu-id="56c6e-372">30105</span><span class="sxs-lookup"><span data-stu-id="56c6e-372">30105</span></span>
<span data-ttu-id="56c6e-373">Личный сайт пользователя в OneDrive для бизнеса не подготовлен к работе. Это необходимо для доступа к записным книжкам.</span><span class="sxs-lookup"><span data-stu-id="56c6e-373">The user's personal OneDrive for Business site is not provisioned, which is required to access notebooks.</span></span> <span data-ttu-id="56c6e-374">Служба OneNote подготовит сайт к работе.</span><span class="sxs-lookup"><span data-stu-id="56c6e-374">The OneNote service will provision the site now.</span></span> <span data-ttu-id="56c6e-375">Этот процесс может занять несколько минут.</span><span class="sxs-lookup"><span data-stu-id="56c6e-375">This process may take several minutes.</span></span>

### <a name="30106"></a><span data-ttu-id="56c6e-376">30106</span><span class="sxs-lookup"><span data-stu-id="56c6e-376">30106</span></span>
<span data-ttu-id="56c6e-377">OneDrive для бизнеса подготавливается к работе для пользователя.</span><span class="sxs-lookup"><span data-stu-id="56c6e-377">OneDrive for Business is being provisioned for the user.</span></span>

### <a name="30108"></a><span data-ttu-id="56c6e-378">30108</span><span class="sxs-lookup"><span data-stu-id="56c6e-378">30108</span></span>
<span data-ttu-id="56c6e-379">Не удалось получить личное хранилище пользователя в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="56c6e-379">The user's personal OneDrive for Business could not be retrieved.</span></span> <span data-ttu-id="56c6e-380">В приведенной ниже таблице перечислены некоторые возможные причины.</span><span class="sxs-lookup"><span data-stu-id="56c6e-380">The following table lists some possible causes.</span></span>

| <span data-ttu-id="56c6e-381">Причина</span><span class="sxs-lookup"><span data-stu-id="56c6e-381">Cause</span></span> | <span data-ttu-id="56c6e-382">Решение</span><span class="sxs-lookup"><span data-stu-id="56c6e-382">Resolution</span></span> |
|:------|:------|
| <span data-ttu-id="56c6e-383">Личный сайт пользователя не подготовлен к работе.</span><span class="sxs-lookup"><span data-stu-id="56c6e-383">The user's personal site has not been provisioned.</span></span> | <span data-ttu-id="56c6e-384">Пользователь должен открыть OneDrive для бизнеса и следовать указаниям по подготовке сайта к работе.</span><span class="sxs-lookup"><span data-stu-id="56c6e-384">The user should open OneDrive for Business and follow any instructions to provision the site.</span></span> <span data-ttu-id="56c6e-385">Если проблема не будет устранена, необходимо обратиться к администратору клиента Office 365.</span><span class="sxs-lookup"><span data-stu-id="56c6e-385">If this fails, they should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="56c6e-386">В данный момент личный сайт пользователя подготавливается к работе.</span><span class="sxs-lookup"><span data-stu-id="56c6e-386">The user's personal site is currently being provisioned.</span></span> | <span data-ttu-id="56c6e-387">Попробуйте отправить запрос позже.</span><span class="sxs-lookup"><span data-stu-id="56c6e-387">Try the request later.</span></span> |
| <span data-ttu-id="56c6e-388">У пользователя нет действительной лицензии на OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="56c6e-388">The user does not have a valid OneDrive for Business license.</span></span> | <span data-ttu-id="56c6e-389">Пользователь должен обратиться к администратору своего клиента Office 365.</span><span class="sxs-lookup"><span data-stu-id="56c6e-389">The user should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="56c6e-390">Не удается отправить запрос из-за проблем с сетью.</span><span class="sxs-lookup"><span data-stu-id="56c6e-390">A network issue prevented the request from being successfully sent.</span></span> | <span data-ttu-id="56c6e-391">Попробуйте отправить запрос позже.</span><span class="sxs-lookup"><span data-stu-id="56c6e-391">Try the request later.</span></span> |

### <a name="30109"></a><span data-ttu-id="56c6e-392">30109</span><span class="sxs-lookup"><span data-stu-id="56c6e-392">30109</span></span>
<span data-ttu-id="56c6e-393">Некоторые пользователи, указанные в запросе, не существуют.</span><span class="sxs-lookup"><span data-stu-id="56c6e-393">Some users in the request do not exist.</span></span>

### <a name="30110"></a><span data-ttu-id="56c6e-394">30110</span><span class="sxs-lookup"><span data-stu-id="56c6e-394">30110</span></span>
<span data-ttu-id="56c6e-395">Для этого клиента не зарегистрированы службы сведений об учащихся.</span><span class="sxs-lookup"><span data-stu-id="56c6e-395">Student Information Services has not been registered for this tenant.</span></span>

### <a name="30111"></a><span data-ttu-id="56c6e-396">30111</span><span class="sxs-lookup"><span data-stu-id="56c6e-396">30111</span></span>
<span data-ttu-id="56c6e-397">Возникла общая ошибка служб сведений об учащихся.</span><span class="sxs-lookup"><span data-stu-id="56c6e-397">There is a generic error with Student Information Services.</span></span>

### <a name="30112"></a><span data-ttu-id="56c6e-398">30112</span><span class="sxs-lookup"><span data-stu-id="56c6e-398">30112</span></span>
<span data-ttu-id="56c6e-399">Запрос влияет на нескольких пользователей с одинаковыми именами.</span><span class="sxs-lookup"><span data-stu-id="56c6e-399">Multiple users affected by the request had the same username.</span></span>

### <a name="30113"></a><span data-ttu-id="56c6e-400">30113</span><span class="sxs-lookup"><span data-stu-id="56c6e-400">30113</span></span>
<span data-ttu-id="56c6e-401">Для записной книжки не разрешены приглашения.</span><span class="sxs-lookup"><span data-stu-id="56c6e-401">The notebook is not configured to allow invites.</span></span>

### <a name="30114"></a><span data-ttu-id="56c6e-402">30114</span><span class="sxs-lookup"><span data-stu-id="56c6e-402">30114</span></span>
<span data-ttu-id="56c6e-403">Отсутствует обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="56c6e-403">There is a required parameter missing.</span></span>

## <a name="codes-from-40001-to-49999"></a><span data-ttu-id="56c6e-404">Коды от 40001 до 49999</span><span class="sxs-lookup"><span data-stu-id="56c6e-404">Codes from 40001 to 49999</span></span>
<span data-ttu-id="56c6e-405">У пользователя или приложения нет необходимых разрешений.</span><span class="sxs-lookup"><span data-stu-id="56c6e-405">The user or application does not have the correct permissions.</span></span>

### <a name="40001"></a><span data-ttu-id="56c6e-406">40001</span><span class="sxs-lookup"><span data-stu-id="56c6e-406">40001</span></span>
<span data-ttu-id="56c6e-407">Запрос не содержит действительный маркер OAuth.</span><span class="sxs-lookup"><span data-stu-id="56c6e-407">The request doesn't contain a valid OAuth token.</span></span> <span data-ttu-id="56c6e-408">См. раздел [Разрешения для заметок](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="56c6e-408">See [Notes permissions](permissions_reference.md#notes-permissions).</span></span>

### <a name="40002"></a><span data-ttu-id="56c6e-409">40002</span><span class="sxs-lookup"><span data-stu-id="56c6e-409">40002</span></span>
<span data-ttu-id="56c6e-410">У пользователя нет разрешения на запись в указанном расположении.</span><span class="sxs-lookup"><span data-stu-id="56c6e-410">The user doesn't have permission to write to the requested location.</span></span>

### <a name="40003"></a><span data-ttu-id="56c6e-411">40003</span><span class="sxs-lookup"><span data-stu-id="56c6e-411">40003</span></span>
<span data-ttu-id="56c6e-412">У пользователя нет разрешения на доступ к запрашиваемому ресурсу.</span><span class="sxs-lookup"><span data-stu-id="56c6e-412">The user doesn't have permission to access the requested resource.</span></span>

### <a name="40004"></a><span data-ttu-id="56c6e-413">40004</span><span class="sxs-lookup"><span data-stu-id="56c6e-413">40004</span></span>
<span data-ttu-id="56c6e-414">Область действия маркера OAuth недостаточна для выполнения запрашиваемого действия.</span><span class="sxs-lookup"><span data-stu-id="56c6e-414">The OAuth token doesn't have the required scopes to perform the requested action.</span></span> <span data-ttu-id="56c6e-415">См. раздел [Разрешения для заметок](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="56c6e-415">See [Notes permissions](permissions_reference.md#notes-permissions).</span></span>

### <a name="40006"></a><span data-ttu-id="56c6e-416">40006</span><span class="sxs-lookup"><span data-stu-id="56c6e-416">40006</span></span> 
<span data-ttu-id="56c6e-417">Область действия маркера OAuth недостаточна для выполнения запрашиваемого действия.</span><span class="sxs-lookup"><span data-stu-id="56c6e-417">The OAuth token doesn't have the required scopes to perform the requested action.</span></span> <span data-ttu-id="56c6e-418">В частности, это относится к разрешению на редактирование.</span><span class="sxs-lookup"><span data-stu-id="56c6e-418">Specifically the edit permission.</span></span> <span data-ttu-id="56c6e-419">См. раздел [Разрешения для заметок](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="56c6e-419">See [Notes permissions](permissions_reference.md#notes-permissions).</span></span>

### <a name="40007"></a><span data-ttu-id="56c6e-420">40007</span><span class="sxs-lookup"><span data-stu-id="56c6e-420">40007</span></span>
<span data-ttu-id="56c6e-421">У пользователя нет разрешений на доступ к этому ресурсу.</span><span class="sxs-lookup"><span data-stu-id="56c6e-421">The user does not have permissions to access this resource.</span></span>

### <a name="40008"></a><span data-ttu-id="56c6e-422">40008</span><span class="sxs-lookup"><span data-stu-id="56c6e-422">40008</span></span>
<span data-ttu-id="56c6e-423">Доступ к этому ресурсу запрещен.</span><span class="sxs-lookup"><span data-stu-id="56c6e-423">Access is Forbidden for this resource.</span></span>

### <a name="40009"></a><span data-ttu-id="56c6e-424">40009</span><span class="sxs-lookup"><span data-stu-id="56c6e-424">40009</span></span>
<span data-ttu-id="56c6e-425">Контейнер уже используется другим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="56c6e-425">The container is already in use by another resource.</span></span>

## <a name="see-also"></a><span data-ttu-id="56c6e-426">См. также</span><span class="sxs-lookup"><span data-stu-id="56c6e-426">See also</span></span>

- [<span data-ttu-id="56c6e-427">Сообщения об ошибках и типы ресурсов ошибок Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="56c6e-427">Microsoft Graph error responses and resource types</span></span>](errors.md)
- [<span data-ttu-id="56c6e-428">Справочник по OneNote</span><span class="sxs-lookup"><span data-stu-id="56c6e-428">OneNote reference</span></span>](../api-reference/v1.0/resources/onenote.md)

