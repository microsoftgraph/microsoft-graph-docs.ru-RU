---
title: Коды ошибок для API OneNote в Microsoft Graph
description: В этой статье описываются коды ошибок, возвращаемые API OneNote в Microsoft Graph при сбоях запросов, отправляемых через API.
ms.openlocfilehash: 265929be081ee61a88b8baf4f600e2c154797ec7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092673"
---
# <a name="error-codes-for-onenote-apis-in-microsoft-graph"></a><span data-ttu-id="e2763-103">Коды ошибок для API OneNote в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e2763-103">Error codes for OneNote APIs in Microsoft Graph</span></span>

<span data-ttu-id="e2763-104">В этой статье описываются коды ошибок, возвращаемые API OneNote в Microsoft Graph при сбоях запросов, отправляемых через API.</span><span class="sxs-lookup"><span data-stu-id="e2763-104">This article describes error codes that are returned by the OneNote APIs in Microsoft Graph whenever a request sent through the API fails.</span></span>

## <a name="error-response-example"></a><span data-ttu-id="e2763-105">Пример ответа об ошибке</span><span class="sxs-lookup"><span data-stu-id="e2763-105">Error response example</span></span>

<span data-ttu-id="e2763-106">Если при отправке запроса возникает ошибка, API OneNote перестает выполнять запрос и возвращает ответ об ошибке в виде объекта JSON.</span><span class="sxs-lookup"><span data-stu-id="e2763-106">When your request generates an error, the OneNote API stops performing the request and returns an error response as a JSON object.</span></span> <span data-ttu-id="e2763-107">Ответ об ошибке содержит соответствующий код ошибки, сообщение и ссылку на соответствующий раздел этой статьи.</span><span class="sxs-lookup"><span data-stu-id="e2763-107">An error response contains the associated error code, a message, and a link to the appropriate section of this article.</span></span> <span data-ttu-id="e2763-108">В приведенном ниже примере показано, как выглядит ответ об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e2763-108">The following example shows how an error response looks.</span></span>

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

<span data-ttu-id="e2763-109">Дополнительные сведения об ошибках Microsoft Graph см. в статье [Сообщения об ошибках и типы ресурсов ошибок Microsoft Graph](errors.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-109">For more information about Microsoft Graph errors, see [Microsoft Graph error responses and resource types](errors.md).</span></span>

## <a name="codes-from-10001-to-19999"></a><span data-ttu-id="e2763-110">Коды от 10001 до 19999</span><span class="sxs-lookup"><span data-stu-id="e2763-110">Codes from 10001 to 19999</span></span>

<span data-ttu-id="e2763-111">Служба работает с ошибками или отправляет информацию в приложение.</span><span class="sxs-lookup"><span data-stu-id="e2763-111">The service is having problems or is sending information to the application.</span></span>

### <a name="10001"></a><span data-ttu-id="e2763-112">10001</span><span class="sxs-lookup"><span data-stu-id="e2763-112">10001</span></span>
<span data-ttu-id="e2763-113">Произошла непредвиденная ошибка, и запрос не выполнен.</span><span class="sxs-lookup"><span data-stu-id="e2763-113">An unexpected error occurred and the request failed.</span></span>

### <a name="10002"></a><span data-ttu-id="e2763-114">10002</span><span class="sxs-lookup"><span data-stu-id="e2763-114">10002</span></span>
<span data-ttu-id="e2763-115">Служба в настоящее время недоступна.</span><span class="sxs-lookup"><span data-stu-id="e2763-115">The service is not currently available.</span></span>

### <a name="10003"></a><span data-ttu-id="e2763-116">10003</span><span class="sxs-lookup"><span data-stu-id="e2763-116">10003</span></span>
<span data-ttu-id="e2763-117">Учетная запись текущего пользователя превысила максимальное число активных запросов.</span><span class="sxs-lookup"><span data-stu-id="e2763-117">The current user's account has exceeded the maximum number of active requests.</span></span> <span data-ttu-id="e2763-118">Приложению придется повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="e2763-118">Your app will have to repeat the request.</span></span>

### <a name="10004"></a><span data-ttu-id="e2763-119">10004</span><span class="sxs-lookup"><span data-stu-id="e2763-119">10004</span></span>
<span data-ttu-id="e2763-120">Служба не может создать страницу в запрашиваемом разделе, так как раздел защищен паролем.</span><span class="sxs-lookup"><span data-stu-id="e2763-120">The service can't create a page in the requested section because that section is protected by a password.</span></span>

### <a name="10005"></a><span data-ttu-id="e2763-121">10005</span><span class="sxs-lookup"><span data-stu-id="e2763-121">10005</span></span>
<span data-ttu-id="e2763-122">В запросе превышено максимальное количество тегов изображений, в которых атрибут **data-render-src** содержит PDF-файл.</span><span class="sxs-lookup"><span data-stu-id="e2763-122">The request contains more than the maximum number of image tags in which the **data-render-src** attribute contains a PDF.</span></span> <span data-ttu-id="e2763-123">См. статью [Добавление изображений и файлов](onenote-images-files.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-123">See [Add images and files](onenote-images-files.md).</span></span>

### <a name="10006"></a><span data-ttu-id="e2763-124">10006</span><span class="sxs-lookup"><span data-stu-id="e2763-124">10006</span></span>
<span data-ttu-id="e2763-125">API OneNote не удалось создать страницу в указанном разделе, потому что раздел поврежден.</span><span class="sxs-lookup"><span data-stu-id="e2763-125">The OneNote API was unable to create a page in the specified section because that section is corrupt.</span></span>

### <a name="10007"></a><span data-ttu-id="e2763-126">10007</span><span class="sxs-lookup"><span data-stu-id="e2763-126">10007</span></span>
<span data-ttu-id="e2763-p104">Сервер слишком занят, чтобы обработать входящий запрос в данный момент. Повторите попытку позже.</span><span class="sxs-lookup"><span data-stu-id="e2763-p104">The server is too busy to handle the incoming request at this moment. Please try again later.</span></span>

### <a name="10008"></a><span data-ttu-id="e2763-129">10008</span><span class="sxs-lookup"><span data-stu-id="e2763-129">10008</span></span>
<span data-ttu-id="e2763-130">Одна или несколько библиотек документов в хранилище OneDrive пользователя или группы содержит более 5000 элементов OneNote (записных книжек, разделов, групп разделов), и к ней невозможно отправлять запросы с помощью API.</span><span class="sxs-lookup"><span data-stu-id="e2763-130">One or more of the document libraries on the user or group's OneDrive contains more than 5000 OneNote items (notebooks, sections, section groups), and cannot be queried using the API.</span></span> <span data-ttu-id="e2763-131">Убедитесь, что ни одна из библиотек документов пользователей и групп не содержит более 5000 элементов OneNote.</span><span class="sxs-lookup"><span data-stu-id="e2763-131">Please make sure that none of the user or group's document libraries contains more than 5000 OneNote items.</span></span> <span data-ttu-id="e2763-132">Указания по устранению этой проблемы см. в [блоге разработчиков OneNote](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/).</span><span class="sxs-lookup"><span data-stu-id="e2763-132">See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10012"></a><span data-ttu-id="e2763-133">10012</span><span class="sxs-lookup"><span data-stu-id="e2763-133">10012</span></span>
<span data-ttu-id="e2763-134">Не удается создать или обновить объект, так как в библиотеке, содержащей записную книжку, требуется получать элементы для изменения, прежде чем редактировать их.</span><span class="sxs-lookup"><span data-stu-id="e2763-134">Unable to create or update the entity because the library that contains the notebook requires items to be checked out before they can be edited.</span></span> <span data-ttu-id="e2763-135">Дополнительные сведения см. в статье [Как включить в библиотеке обязательное извлечение файлов](https://support.office.com/ru-RU/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7).</span><span class="sxs-lookup"><span data-stu-id="e2763-135">For more information, see [Set up a library to require check-out of files](https://support.office.com/ru-RU/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7).</span></span>

<span data-ttu-id="e2763-136">Отмените обязательное извлечение для этой библиотеки или переместите записную книжку.</span><span class="sxs-lookup"><span data-stu-id="e2763-136">Either remove the check-out requirement from the library, or move the notebook.</span></span>

### <a name="10013"></a><span data-ttu-id="e2763-137">10013</span><span class="sxs-lookup"><span data-stu-id="e2763-137">10013</span></span>
<span data-ttu-id="e2763-p107">Одна или более библиотек документов в OneDrive пользователя или группы содержит более 20 000 элементов и не может быть индексирована по запросу с помощью API. Убедитесь, что ни одна из библиотек документов пользователя или группы не содержит более 20 000 элементов. Действия по устранению рисков см. в [блоге разработчиков OneNote Dev](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/).</span><span class="sxs-lookup"><span data-stu-id="e2763-p107">One or more of the document libraries on the user or group's OneDrive contains more than 5000 OneNote items (notebooks, sections, section groups), and cannot be queried using the API. Please make sure that none of the user or group's document libraries contains more than 5000 OneNote items. See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10014"></a><span data-ttu-id="e2763-141">10014</span><span class="sxs-lookup"><span data-stu-id="e2763-141">10014</span></span>
<span data-ttu-id="e2763-142">В данный момент служба Azure Key Vault слишком занята для обработки входящего запроса.</span><span class="sxs-lookup"><span data-stu-id="e2763-142">Azure Key Vault is too busy to handle the incoming request at this moment.</span></span> <span data-ttu-id="e2763-143">Повторите попытку позже.</span><span class="sxs-lookup"><span data-stu-id="e2763-143">Please try again later.</span></span>

### <a name="10015"></a><span data-ttu-id="e2763-144">10015</span><span class="sxs-lookup"><span data-stu-id="e2763-144">10015</span></span>
<span data-ttu-id="e2763-145">В настоящее время среда SharePoint недоступна.</span><span class="sxs-lookup"><span data-stu-id="e2763-145">SharePoint is currently unavailable.</span></span> <span data-ttu-id="e2763-146">Повторите попытку позже.</span><span class="sxs-lookup"><span data-stu-id="e2763-146">Please try again later.</span></span>

### <a name="10016"></a><span data-ttu-id="e2763-147">10016</span><span class="sxs-lookup"><span data-stu-id="e2763-147">10016</span></span>
<span data-ttu-id="e2763-148">Библиотека документов в хранилище OneDrive пользователя или группы превысила пороговое количество уникальных областей безопасности.</span><span class="sxs-lookup"><span data-stu-id="e2763-148">Document library on the user or group’s OneDrive exceeded unique security scopes threshold limit.</span></span> <span data-ttu-id="e2763-149">Число уникальных областей безопасности для каждой библиотеки не может превышать 50 000.</span><span class="sxs-lookup"><span data-stu-id="e2763-149">The maximum number of unique security scopes set for a library cannot exceed 50,000.</span></span>

### <a name="10017"></a><span data-ttu-id="e2763-150">10017</span><span class="sxs-lookup"><span data-stu-id="e2763-150">10017</span></span>
<span data-ttu-id="e2763-151">Неправильный запрос.</span><span class="sxs-lookup"><span data-stu-id="e2763-151">Bad Request.</span></span>

### <a name="19999"></a><span data-ttu-id="e2763-152">19999</span><span class="sxs-lookup"><span data-stu-id="e2763-152">19999</span></span>
<span data-ttu-id="e2763-153">Запрос не выполнен из-за неизвестной ошибки.</span><span class="sxs-lookup"><span data-stu-id="e2763-153">The request failed because an undetermined error occurred.</span></span>

## <a name="codes-from-20001-to-29999"></a><span data-ttu-id="e2763-154">Коды от 20001 до 29999</span><span class="sxs-lookup"><span data-stu-id="e2763-154">Codes from 20001 to 29999</span></span>

<span data-ttu-id="e2763-155">Код приложения допустил ошибку.</span><span class="sxs-lookup"><span data-stu-id="e2763-155">The application code has done something wrong.</span></span>

### <a name="20001"></a><span data-ttu-id="e2763-156">20001</span><span class="sxs-lookup"><span data-stu-id="e2763-156">20001</span></span>

<span data-ttu-id="e2763-157">В запросе отсутствует необходимый раздел Presentation.</span><span class="sxs-lookup"><span data-stu-id="e2763-157">The request is missing the required "Presentation" part.</span></span> <span data-ttu-id="e2763-158">Он должен быть только один.</span><span class="sxs-lookup"><span data-stu-id="e2763-158">Exactly one is required.</span></span> 

### <a name="20002"></a><span data-ttu-id="e2763-159">20002</span><span class="sxs-lookup"><span data-stu-id="e2763-159">20002</span></span>
<span data-ttu-id="e2763-160">Запрос содержит две или более части Presentation.</span><span class="sxs-lookup"><span data-stu-id="e2763-160">The request contains two or more "Presentation" parts.</span></span> <span data-ttu-id="e2763-161">Он должен быть только один.</span><span class="sxs-lookup"><span data-stu-id="e2763-161">Exactly one is required.</span></span>

### <a name="20003"></a><span data-ttu-id="e2763-162">20003</span><span class="sxs-lookup"><span data-stu-id="e2763-162">20003</span></span>
<span data-ttu-id="e2763-163">В разделе Presentation допускаются только типы контента text/HTML и application/XHTML+XML.</span><span class="sxs-lookup"><span data-stu-id="e2763-163">The content type of the "Presentation" part can be only text/HTML or application/XHTML+XML.</span></span> 

### <a name="20004"></a><span data-ttu-id="e2763-164">20004</span><span class="sxs-lookup"><span data-stu-id="e2763-164">20004</span></span>
<span data-ttu-id="e2763-p113">HTML-код части "Presentation" содержит тег изображения с обоими наборами свойств: **src** и **data-render-src**. API будет игнорировать свойство **src** и использовать свойство **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="e2763-p113">The "Presentation" part HTML contains an image tag with both the **src** and the **data-render-src** properties set. The API will ignore the **src** property and use the **data-render-src** property. See OneNote API reference.</span></span> 

### <a name="20005"></a><span data-ttu-id="e2763-167">20005</span><span class="sxs-lookup"><span data-stu-id="e2763-167">20005</span></span>
<span data-ttu-id="e2763-168">URI запроса слишком длинный.</span><span class="sxs-lookup"><span data-stu-id="e2763-168">The request URI is too long.</span></span> <span data-ttu-id="e2763-169">Максимальный размер URI (включая все параметры и данные) составляет 16 КБ или 16 384 символов.</span><span class="sxs-lookup"><span data-stu-id="e2763-169">The maximum size of the URI (including all parameters and data) is 16 KB or 16,384 characters.</span></span>

### <a name="20006"></a><span data-ttu-id="e2763-170">20006</span><span class="sxs-lookup"><span data-stu-id="e2763-170">20006</span></span>
<span data-ttu-id="e2763-171">HTML-код раздела Presentation содержит тег image, в котором не заданы свойства src и **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="e2763-171">The "Presentation" part HTML contains an image tag with neither the src nor the **data-render-src** properties set.</span></span> <span data-ttu-id="e2763-172">API проигнорирует тег **image**.</span><span class="sxs-lookup"><span data-stu-id="e2763-172">The API will ignore the **image** tag.</span></span> 

### <a name="20007"></a><span data-ttu-id="e2763-173">20007</span><span class="sxs-lookup"><span data-stu-id="e2763-173">20007</span></span>
<span data-ttu-id="e2763-174">HTML-код раздела Presentation содержит строку даты и времени создания, которая не соответствует ни одному из допустимых форматов.</span><span class="sxs-lookup"><span data-stu-id="e2763-174">The "Presentation" part HTML contains a created date/time string that does not match any of the allowed formats.</span></span> 

### <a name="20008"></a><span data-ttu-id="e2763-175">20008</span><span class="sxs-lookup"><span data-stu-id="e2763-175">20008</span></span>
<span data-ttu-id="e2763-176">Размер запроса превышает допустимый.</span><span class="sxs-lookup"><span data-stu-id="e2763-176">The size of the request is too large.</span></span> 

### <a name="20009"></a><span data-ttu-id="e2763-177">20009</span><span class="sxs-lookup"><span data-stu-id="e2763-177">20009</span></span>
<span data-ttu-id="e2763-178">Запрос содержит разделы с повторяющимися именами.</span><span class="sxs-lookup"><span data-stu-id="e2763-178">The request contains parts with duplicate names.</span></span> <span data-ttu-id="e2763-179">Имена разделов должны быть уникальными.</span><span class="sxs-lookup"><span data-stu-id="e2763-179">Part names must be unique.</span></span> 

### <a name="20010"></a><span data-ttu-id="e2763-180">20010</span><span class="sxs-lookup"><span data-stu-id="e2763-180">20010</span></span>
<span data-ttu-id="e2763-181">Для указанного типа контента не предоставлен заголовок Content-Disposition.</span><span class="sxs-lookup"><span data-stu-id="e2763-181">The Content-Disposition header was not supplied for the specified content type.</span></span> 

### <a name="20011"></a><span data-ttu-id="e2763-182">20011</span><span class="sxs-lookup"><span data-stu-id="e2763-182">20011</span></span>
<span data-ttu-id="e2763-183">Запрос содержит составные полезные данные неправильного формата.</span><span class="sxs-lookup"><span data-stu-id="e2763-183">The request contains a malformed multipart payload.</span></span> <span data-ttu-id="e2763-184">К возможным причинам этой ошибки относятся пустые строки, отсутствие последней строки, неправильно отформатированные разделители частей и т. д.</span><span class="sxs-lookup"><span data-stu-id="e2763-184">Problems could include missing blank lines, a missing last line, incorrectly formatted part separators, and so on.</span></span> <span data-ttu-id="e2763-185">Если вы создаете составное сообщение вручную, внимательно проверьте логику или используйте стороннюю библиотеку.</span><span class="sxs-lookup"><span data-stu-id="e2763-185">If you're building the multipart message by hand, carefully check the logic, or consider using a third-party library.</span></span> 

### <a name="20012"></a><span data-ttu-id="e2763-186">20012</span><span class="sxs-lookup"><span data-stu-id="e2763-186">20012</span></span>
<span data-ttu-id="e2763-187">В запросе не предоставлен тип контента для указанной части.</span><span class="sxs-lookup"><span data-stu-id="e2763-187">The request doesn't supply a content type for the specified part.</span></span> 

### <a name="20013"></a><span data-ttu-id="e2763-188">20013</span><span class="sxs-lookup"><span data-stu-id="e2763-188">20013</span></span>
<span data-ttu-id="e2763-189">В запросе не предоставлены заголовки Content-Type и Content-Disposition для указанной части.</span><span class="sxs-lookup"><span data-stu-id="e2763-189">The request doesn't supply Content-Type and Content-Disposition headers for the specified part.</span></span> 

### <a name="20014"></a><span data-ttu-id="e2763-190">20014</span><span class="sxs-lookup"><span data-stu-id="e2763-190">20014</span></span>
<span data-ttu-id="e2763-191">Длина части составного сообщения превышает максимальную (25 МБ).</span><span class="sxs-lookup"><span data-stu-id="e2763-191">The length of a part in the multipart message exceeds the maximum size of 25 MB.</span></span> 

### <a name="20015"></a><span data-ttu-id="e2763-192">20015</span><span class="sxs-lookup"><span data-stu-id="e2763-192">20015</span></span>
<span data-ttu-id="e2763-193">Количество частей составного сообщения превышает максимальное (500).</span><span class="sxs-lookup"><span data-stu-id="e2763-193">The count of parts in the multipart message exceeds the limit of 500.</span></span> 

### <a name="20016"></a><span data-ttu-id="e2763-194">20016</span><span class="sxs-lookup"><span data-stu-id="e2763-194">20016</span></span>
<span data-ttu-id="e2763-195">Длина составного сообщения превышает максимальную (75 МБ).</span><span class="sxs-lookup"><span data-stu-id="e2763-195">The length of the multipart message exceeds the limit of 75 MB.</span></span> 

### <a name="20017"></a><span data-ttu-id="e2763-196">20017</span><span class="sxs-lookup"><span data-stu-id="e2763-196">20017</span></span>
<span data-ttu-id="e2763-197">Неправильный формат MIME электронного сообщения.</span><span class="sxs-lookup"><span data-stu-id="e2763-197">The email MIME was malformed.</span></span> 

### <a name="20018"></a><span data-ttu-id="e2763-198">20018</span><span class="sxs-lookup"><span data-stu-id="e2763-198">20018</span></span>
<span data-ttu-id="e2763-199">Неправильный формат MIME или элемента ICal для собрания.</span><span class="sxs-lookup"><span data-stu-id="e2763-199">The meeting MIME or ICal was malformed.</span></span> 

### <a name="20019"></a><span data-ttu-id="e2763-200">20019</span><span class="sxs-lookup"><span data-stu-id="e2763-200">20019</span></span>
<span data-ttu-id="e2763-201">Элемент ICal не найден.</span><span class="sxs-lookup"><span data-stu-id="e2763-201">No ICal was found.</span></span> 

### <a name="20020"></a><span data-ttu-id="e2763-202">20020</span><span class="sxs-lookup"><span data-stu-id="e2763-202">20020</span></span>
<span data-ttu-id="e2763-203">В теле запроса обнаружен объект JSON неправильного формата.</span><span class="sxs-lookup"><span data-stu-id="e2763-203">Encountered malformed Json in request body.</span></span> 

### <a name="20100"></a><span data-ttu-id="e2763-204">20100</span><span class="sxs-lookup"><span data-stu-id="e2763-204">20100</span></span>
<span data-ttu-id="e2763-205">Ошибка синтаксиса запроса.</span><span class="sxs-lookup"><span data-stu-id="e2763-205">Something is wrong with the syntax of your request.</span></span> 

### <a name="20101"></a><span data-ttu-id="e2763-206">20101</span><span class="sxs-lookup"><span data-stu-id="e2763-206">20101</span></span>
<span data-ttu-id="e2763-207">Запрашиваемое свойство не существует.</span><span class="sxs-lookup"><span data-stu-id="e2763-207">The property that you requested doesn't exist.</span></span>

### <a name="20102"></a><span data-ttu-id="e2763-208">20102</span><span class="sxs-lookup"><span data-stu-id="e2763-208">20102</span></span>
<span data-ttu-id="e2763-209">Запрашиваемый ресурс не существует.</span><span class="sxs-lookup"><span data-stu-id="e2763-209">You requested a resource that doesn't exist.</span></span>

### <a name="20103"></a><span data-ttu-id="e2763-210">20103</span><span class="sxs-lookup"><span data-stu-id="e2763-210">20103</span></span>
<span data-ttu-id="e2763-211">Оператор **expand** не поддерживается для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="e2763-211">The **expand** query is not supported for this request.</span></span> <span data-ttu-id="e2763-212">См. раздел [Поддерживаемые параметры строки запроса OData](onenote-get-content.md#supported-odata-query-string-options).</span><span class="sxs-lookup"><span data-stu-id="e2763-212">See [Supported OData query string options](onenote-get-content.md#supported-odata-query-string-options).</span></span>

### <a name="20104"></a><span data-ttu-id="e2763-213">20104</span><span class="sxs-lookup"><span data-stu-id="e2763-213">20104 (SectionNameInvalidChar)</span></span>
<span data-ttu-id="e2763-p119">Параметр запроса **pagelevel** поддерживается только для запроса коллекции страниц в разделе или конкретной страницы. Например:</span><span class="sxs-lookup"><span data-stu-id="e2763-p119">The **pagelevel** query option is supported only when querying for the pages collection in a section or for a specific page. For example:</span></span>  

```http
GET ../sections/{id}/pages?pagelevel=true
GET ../pages/{id}?pagelevel=true
```

### <a name="20106"></a><span data-ttu-id="e2763-216">20106</span><span class="sxs-lookup"><span data-stu-id="e2763-216">20106</span></span>
<span data-ttu-id="e2763-217">Запрос содержит неподдерживаемый оператор.</span><span class="sxs-lookup"><span data-stu-id="e2763-217">Your request contains a query operator that is not supported.</span></span> 

### <a name="20108"></a><span data-ttu-id="e2763-218">20108</span><span class="sxs-lookup"><span data-stu-id="e2763-218">20108</span></span>
<span data-ttu-id="e2763-219">Запрос содержит неподдерживаемые параметры запроса OData.</span><span class="sxs-lookup"><span data-stu-id="e2763-219">Your request contains unsupported OData query parameters.</span></span>

### <a name="20109"></a><span data-ttu-id="e2763-220">20109</span><span class="sxs-lookup"><span data-stu-id="e2763-220">20109</span></span>
<span data-ttu-id="e2763-221">Полезные данные в PATCH-запросе неправильно построены.</span><span class="sxs-lookup"><span data-stu-id="e2763-221">The payload in the PATCH request is not constructed correctly.</span></span>

### <a name="20110"></a><span data-ttu-id="e2763-222">20110</span><span class="sxs-lookup"><span data-stu-id="e2763-222">20110</span></span>
<span data-ttu-id="e2763-223">Для запросов на создание страниц с частями данных необходимо составное содержимое с разделом Presentation.</span><span class="sxs-lookup"><span data-stu-id="e2763-223">Page create requests with data parts require the content to be multipart, with a "Presentation" part.</span></span> 

### <a name="20111"></a><span data-ttu-id="e2763-224">20111</span><span class="sxs-lookup"><span data-stu-id="e2763-224">20111</span></span>
<span data-ttu-id="e2763-225">В запросе используется неподдерживаемая функция OData.</span><span class="sxs-lookup"><span data-stu-id="e2763-225">Your request uses an OData feature that isn't supported.</span></span>

### <a name="20112"></a><span data-ttu-id="e2763-226">20112</span><span class="sxs-lookup"><span data-stu-id="e2763-226">20112</span></span>
<span data-ttu-id="e2763-227">Запрос содержит недопустимый идентификатор для целевой сущности записной книжки, группы разделов, раздела или страницы.</span><span class="sxs-lookup"><span data-stu-id="e2763-227">Your request contains an invalid ID for the target notebook, section group, section, or page entity.</span></span>

### <a name="20113"></a><span data-ttu-id="e2763-228">20113</span><span class="sxs-lookup"><span data-stu-id="e2763-228">20113</span></span>
<span data-ttu-id="e2763-229">Ресурс, заданный в запросе, был удален.</span><span class="sxs-lookup"><span data-stu-id="e2763-229">The resource specified in the request has been deleted.</span></span>

### <a name="20115"></a><span data-ttu-id="e2763-230">20115</span><span class="sxs-lookup"><span data-stu-id="e2763-230">20115</span></span>
<span data-ttu-id="e2763-231">Имя содержит недопустимые символы.</span><span class="sxs-lookup"><span data-stu-id="e2763-231">The name contains invalid characters.</span></span> <span data-ttu-id="e2763-232">Имя записной книжки не может содержать следующие символы: `? * \ / : < > | ' "`</span><span class="sxs-lookup"><span data-stu-id="e2763-232">A notebook name cannot contain any of the following characters: `? * \ / : < > | ' "`</span></span>

### <a name="20117"></a><span data-ttu-id="e2763-233">20117</span><span class="sxs-lookup"><span data-stu-id="e2763-233">20117</span></span>
<span data-ttu-id="e2763-234">Элемент с таким именем уже существует в указанном месте.</span><span class="sxs-lookup"><span data-stu-id="e2763-234">An item with the name you specified already exists in the location that you specified.</span></span>

### <a name="20119"></a><span data-ttu-id="e2763-235">20119</span><span class="sxs-lookup"><span data-stu-id="e2763-235">20119</span></span>
<span data-ttu-id="e2763-236">HTML-код в разделе Presentation содержит атрибут **data-attachment**, который либо неправильно отформатирован либо содержит какие-либо из следующих недопустимых символов для имени файла: `\ / : * ? < > | "`.</span><span class="sxs-lookup"><span data-stu-id="e2763-236">The HTML in the "Presentation" part contains a **data-attachment** attribute that either doesn't have a valid format or includes one or more of these invalid characters for a file name: `\ / : * ? < > | "`.</span></span> <span data-ttu-id="e2763-237">Запрос заменил значение, указанное в сообщении об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e2763-237">The request substituted the value indicated in the error message.</span></span>

### <a name="20120"></a><span data-ttu-id="e2763-238">20120</span><span class="sxs-lookup"><span data-stu-id="e2763-238">20120</span></span>
<span data-ttu-id="e2763-239">В запросе указан целевой объект операции PATCH, который не удается найти.</span><span class="sxs-lookup"><span data-stu-id="e2763-239">Your request specifies a PATCH target that can't be located.</span></span>

### <a name="20121"></a><span data-ttu-id="e2763-240">20121</span><span class="sxs-lookup"><span data-stu-id="e2763-240">20121</span></span>
<span data-ttu-id="e2763-p122">Запрос содержит недопустимый аргумент PATCH. См. статью [Обновление содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-p122">Your request contains an invalid PATCH argument. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20122"></a><span data-ttu-id="e2763-243">20122</span><span class="sxs-lookup"><span data-stu-id="e2763-243">20122</span></span>
<span data-ttu-id="e2763-p123">В запросе указано неподдерживаемое действие PATCH. См. статью [Обновление содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-p123">Your request specifies an unsupported PATCH action. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20123"></a><span data-ttu-id="e2763-246">20123</span><span class="sxs-lookup"><span data-stu-id="e2763-246">20123</span></span>
<span data-ttu-id="e2763-247">PATCH-запросу не удается изменить указанную страницу.</span><span class="sxs-lookup"><span data-stu-id="e2763-247">The PATCH request is unable to alter the specified page.</span></span>

### <a name="20124"></a><span data-ttu-id="e2763-248">20124</span><span class="sxs-lookup"><span data-stu-id="e2763-248">20124</span></span>
<span data-ttu-id="e2763-249">Составной запрос PATCH не содержит раздела commands со структурой JSON действия PATCH.</span><span class="sxs-lookup"><span data-stu-id="e2763-249">Your multipart PATCH request doesn't include a "commands" part with the PATCH action JSON structure.</span></span> <span data-ttu-id="e2763-250">См. статью [Обновление содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-250">See [Update page content](onenote-update-page.md).</span></span>

### <a name="20125"></a><span data-ttu-id="e2763-251">20125</span><span class="sxs-lookup"><span data-stu-id="e2763-251">20125</span></span>
<span data-ttu-id="e2763-p125">В PATCH-запросе не указаны никакие действия. См. статью [Обновление содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-p125">Your PATCH request contains no actions. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20126"></a><span data-ttu-id="e2763-254">20126</span><span class="sxs-lookup"><span data-stu-id="e2763-254">20126</span></span>
<span data-ttu-id="e2763-255">Текст сообщения содержит неправильно отформатированный JSON или поля, неподдерживаемые для этой операции.</span><span class="sxs-lookup"><span data-stu-id="e2763-255">The message body contains either incorrectly formatted JSON or fields that are not supported for this operation.</span></span>

### <a name="20127"></a><span data-ttu-id="e2763-256">20127</span><span class="sxs-lookup"><span data-stu-id="e2763-256">20127</span></span>
<span data-ttu-id="e2763-257">Запрос указывает имя неизвестного свойства.</span><span class="sxs-lookup"><span data-stu-id="e2763-257">Your request specifies the name of an unknown property.</span></span>

### <a name="20128"></a><span data-ttu-id="e2763-258">20128</span><span class="sxs-lookup"><span data-stu-id="e2763-258">20128</span></span>
<span data-ttu-id="e2763-259">Запрос содержит ошибку синтаксиса OData в месте, указанном в сообщении.</span><span class="sxs-lookup"><span data-stu-id="e2763-259">Your request contains an OData syntax error at the position indicated in the message.</span></span>

### <a name="20129"></a><span data-ttu-id="e2763-260">20129</span><span class="sxs-lookup"><span data-stu-id="e2763-260">20129</span></span>
<span data-ttu-id="e2763-261">Запрос содержит параметр строки запроса **top** со слишком большим значением.</span><span class="sxs-lookup"><span data-stu-id="e2763-261">Your request contains a **top** query string option whose value is too high.</span></span> <span data-ttu-id="e2763-262">Для запросов страниц максимальное значение составляет 100, а значение по умолчанию — 20.</span><span class="sxs-lookup"><span data-stu-id="e2763-262">For page queries, the maximum value is 100, and the default value is 20.</span></span>

### <a name="20130"></a><span data-ttu-id="e2763-263">20130</span><span class="sxs-lookup"><span data-stu-id="e2763-263">20130</span></span>
<span data-ttu-id="e2763-264">Запрос содержит URI, указывающий на HTTP-ресурс, который не удается найти.</span><span class="sxs-lookup"><span data-stu-id="e2763-264">Your request contains a URI that points to an HTTP resource that can't be found.</span></span>

### <a name="20131"></a><span data-ttu-id="e2763-265">20131</span><span class="sxs-lookup"><span data-stu-id="e2763-265">20131</span></span>
<span data-ttu-id="e2763-266">Запрос содержит недопустимое значение Content-Type.</span><span class="sxs-lookup"><span data-stu-id="e2763-266">Your request contains an invalid value for Content-Type.</span></span> <span data-ttu-id="e2763-267">Используйте значение, указанное в сообщении.</span><span class="sxs-lookup"><span data-stu-id="e2763-267">Use the value indicated in the message.</span></span> 

### <a name="20132"></a><span data-ttu-id="e2763-268">20132</span><span class="sxs-lookup"><span data-stu-id="e2763-268">20132</span></span>
<span data-ttu-id="e2763-269">Запрос содержит недопустимый контент.</span><span class="sxs-lookup"><span data-stu-id="e2763-269">Your request contains invalid content.</span></span> <span data-ttu-id="e2763-270">Распространенные причины этой проблемы — отсутствие заголовка запроса Content-Type и/или отсутствие содержимого в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="e2763-270">Common causes for this are a missing Content-Type request header and/or no content in the body of the request.</span></span> 

### <a name="20133"></a><span data-ttu-id="e2763-271">20133</span><span class="sxs-lookup"><span data-stu-id="e2763-271">20133</span></span>
<span data-ttu-id="e2763-272">В запросе указан неподдерживаемый целевой объект операции PATCH.</span><span class="sxs-lookup"><span data-stu-id="e2763-272">Your request specifies a PATCH target that is not supported.</span></span> <span data-ttu-id="e2763-273">См. статью [Обновление содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-273">See [Update page content](onenote-update-page.md).</span></span>

### <a name="20134"></a><span data-ttu-id="e2763-274">20134</span><span class="sxs-lookup"><span data-stu-id="e2763-274">20134</span></span>
<span data-ttu-id="e2763-p130">В запросе указан недопустимый элемент в качестве целевого объекта для действия PATCH. Если для целевого объекта используется идентификатор **data-id**, убедитесь, что перед ним указан символ #. См. статью [Обновление содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-p130">Your request specifies an invalid element as the target of the PATCH action. If the target uses the **data-id** identifier, make sure it's prefixed with a # symbol. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20135"></a><span data-ttu-id="e2763-278">20135</span><span class="sxs-lookup"><span data-stu-id="e2763-278">20135</span></span>
<span data-ttu-id="e2763-279">В запросе указан тип объекта, не поддерживаемый для операции PATCH.</span><span class="sxs-lookup"><span data-stu-id="e2763-279">Your request specifies an entity type that is not supported for the PATCH operation.</span></span> <span data-ttu-id="e2763-280">См. статью [Обновление содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-280">See [Update page content](onenote-update-page.md).</span></span>

### <a name="20136"></a><span data-ttu-id="e2763-281">20136</span><span class="sxs-lookup"><span data-stu-id="e2763-281">20136</span></span>
<span data-ttu-id="e2763-282">Запрос содержит недопустимый атрибут **data-render-src** или **data-render-method**, либо этот атрибут отсутствует.</span><span class="sxs-lookup"><span data-stu-id="e2763-282">Your request contains an invalid or missing **data-render-src** or **data-render-method** attribute.</span></span> <span data-ttu-id="e2763-283">См. статью [Извлечение данных из записей](onenote-extract-data.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-283">See [Extract data from captures](onenote-extract-data.md).</span></span>

### <a name="20137"></a><span data-ttu-id="e2763-284">20137</span><span class="sxs-lookup"><span data-stu-id="e2763-284">20137</span></span>
<span data-ttu-id="e2763-285">Конечная страница не поддерживает PATCH-запросы.</span><span class="sxs-lookup"><span data-stu-id="e2763-285">The target page does not support PATCH requests.</span></span>

### <a name="20138"></a><span data-ttu-id="e2763-286">20138</span><span class="sxs-lookup"><span data-stu-id="e2763-286">20138</span></span>
<span data-ttu-id="e2763-p133">Целевой тип элемента в PATCH-запросе не поддерживает действие **append**. См. статью [Обновление содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-p133">The target element type in your PATCH request doesn't support the **append** action. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20139"></a><span data-ttu-id="e2763-289">20139</span><span class="sxs-lookup"><span data-stu-id="e2763-289">20139</span></span>
<span data-ttu-id="e2763-p134">Запрос содержит недопустимое значение атрибута **data-tag**. См. раздел [Использование тегов заметки](onenote-note-tags.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-p134">Your request contains an invalid **data-tag** attribute value. See [Use note tags](onenote-note-tags.md).</span></span>

### <a name="20140"></a><span data-ttu-id="e2763-292">20140</span><span class="sxs-lookup"><span data-stu-id="e2763-292">20140</span></span>
<span data-ttu-id="e2763-293">Запрос содержит недопустимое значение состояния **data-tag**.</span><span class="sxs-lookup"><span data-stu-id="e2763-293">Your request contains an invalid **data-tag** status value.</span></span> <span data-ttu-id="e2763-294">Теги заметок для флажков могут находиться в состоянии **completed**.</span><span class="sxs-lookup"><span data-stu-id="e2763-294">Check box note tags can have a **completed** status.</span></span> 

<span data-ttu-id="e2763-295">Пример.</span><span class="sxs-lookup"><span data-stu-id="e2763-295">Example:</span></span>

```html
    <p data-tag="to-do:completed">To-do note tag in completed state (checked box in the UI)</p>
```
<span data-ttu-id="e2763-296">См. статью [Использование тегов заметок](onenote-note-tags.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-296">See [Use note tags](onenote-note-tags.md).</span></span>

### <a name="20141"></a><span data-ttu-id="e2763-297">20141</span><span class="sxs-lookup"><span data-stu-id="e2763-297">20141</span></span>
<span data-ttu-id="e2763-298">Целевой объект в запросе PATCH не поддерживает указанное действие.</span><span class="sxs-lookup"><span data-stu-id="e2763-298">The target in your PATCH request doesn't support the specified action.</span></span> <span data-ttu-id="e2763-299">См. статью [Обновление содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-299">See [Update page content](onenote-update-page.md).</span></span>

### <a name="20142"></a><span data-ttu-id="e2763-300">20142</span><span class="sxs-lookup"><span data-stu-id="e2763-300">20142</span></span>
<span data-ttu-id="e2763-301">Запрос содержит выражение **expand** для родительского объекта дочерних сущностей или дочернего объекта родительских сущностей. Такие выражения не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="e2763-301">Your request contains an **expand** expression for a parent of child entities or a child of parent entities, which is not supported.</span></span> <span data-ttu-id="e2763-302">См. раздел [Поддерживаемые параметры строки запроса OData](onenote-get-content.md#supported-odata-query-string-options).</span><span class="sxs-lookup"><span data-stu-id="e2763-302">See [Supported OData query string options](onenote-get-content.md#supported-odata-query-string-options).</span></span>

### <a name="20143"></a><span data-ttu-id="e2763-303">20143</span><span class="sxs-lookup"><span data-stu-id="e2763-303">20143</span></span>
<span data-ttu-id="e2763-304">Недопустимый запрос OData.</span><span class="sxs-lookup"><span data-stu-id="e2763-304">The OData query is invalid.</span></span>

### <a name="20144"></a><span data-ttu-id="e2763-305">20144</span><span class="sxs-lookup"><span data-stu-id="e2763-305">20144</span></span>
<span data-ttu-id="e2763-306">Запрос содержит выражение **expand** для свойства, не связанного с навигацией.</span><span class="sxs-lookup"><span data-stu-id="e2763-306">Your request contains an **expand** expression for a non-navigation property.</span></span> <span data-ttu-id="e2763-307">Расширять можно только свойства навигации.</span><span class="sxs-lookup"><span data-stu-id="e2763-307">Only navigation properties can be expanded.</span></span>

### <a name="20145"></a><span data-ttu-id="e2763-308">20145</span><span class="sxs-lookup"><span data-stu-id="e2763-308">20145</span></span>
<span data-ttu-id="e2763-309">Запрос содержит выражение **select** или **expand** с недопустимым термином.</span><span class="sxs-lookup"><span data-stu-id="e2763-309">The **select** or **expand** expression in your request contains an invalid term.</span></span>

### <a name="20146"></a><span data-ttu-id="e2763-310">20146</span><span class="sxs-lookup"><span data-stu-id="e2763-310">20146</span></span>
<span data-ttu-id="e2763-311">Для элемента указан атрибут `style="position:absolute"`, но в элементе **body** не указан атрибут `data-absolute-enabled="true"`, необходимый для поддержки позиционирования.</span><span class="sxs-lookup"><span data-stu-id="e2763-311">The `style="position:absolute"` attribute is specified on an element, but the **body** element does not specify `data-absolute-enabled="true"`, which is required to support positioning.</span></span> <span data-ttu-id="e2763-312">Все параметры положения будут игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="e2763-312">All position settings will be ignored.</span></span> <span data-ttu-id="e2763-313">См. статью [Создание элементов с абсолютным положением](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-313">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20147"></a><span data-ttu-id="e2763-314">20147</span><span class="sxs-lookup"><span data-stu-id="e2763-314">20147</span></span>
<span data-ttu-id="e2763-315">Атрибут `style="position:absolute"` указан для элемента, не являющегося непосредственным дочерним объектом элемента **body**. Этот атрибут не поддерживается для таких элементов.</span><span class="sxs-lookup"><span data-stu-id="e2763-315">The `style="position:absolute"` attribute is specified on an element that is not a direct child of the **body** element, which is not supported.</span></span> <span data-ttu-id="e2763-316">Если это элемент **div**, **img** или **object**, сделайте его непосредственным дочерним объектом основного текста. В противном случае параметры положения будут проигнорированы, а содержимое будет отображаться внутри разделителя с абсолютным положением.</span><span class="sxs-lookup"><span data-stu-id="e2763-316">If the element is a **div**, **img**, or **object**, make it a direct child of the body; otherwise the position settings will be ignored and its content will render inside an absolute positioned div.</span></span> <span data-ttu-id="e2763-317">См. статью [Создание элементов с абсолютным положением](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-317">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20148"></a><span data-ttu-id="e2763-318">20148</span><span class="sxs-lookup"><span data-stu-id="e2763-318">20148</span></span>
<span data-ttu-id="e2763-319">Атрибут `style="position:absolute"` указан для элемента, тип которого не поддерживает этот атрибут.</span><span class="sxs-lookup"><span data-stu-id="e2763-319">The `style="position:absolute"` attribute is specified on an element type that does not support it.</span></span> <span data-ttu-id="e2763-320">Позиционирование поддерживается только для элементов **div**, **img** и **object**, являющихся непосредственными дочерними элементами основного текста.</span><span class="sxs-lookup"><span data-stu-id="e2763-320">Only **div**, **img**, and **object** elements that are direct children of the page body support positioning.</span></span> <span data-ttu-id="e2763-321">См. статью [Создание элементов с абсолютным положением](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="e2763-321">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20149"></a><span data-ttu-id="e2763-322">20149</span><span class="sxs-lookup"><span data-stu-id="e2763-322">20149</span></span>
<span data-ttu-id="e2763-323">Запрос указывает целевой элемент, который не удается найти.</span><span class="sxs-lookup"><span data-stu-id="e2763-323">Your request specifies a target element that cannot be found.</span></span>

### <a name="20150"></a><span data-ttu-id="e2763-324">20150</span><span class="sxs-lookup"><span data-stu-id="e2763-324">20150</span></span>
<span data-ttu-id="e2763-325">Недопустимый запрос для этого типа проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e2763-325">The request is not valid for this authentication type.</span></span> <span data-ttu-id="e2763-326">Используйте путь `../me/onenote/`.</span><span class="sxs-lookup"><span data-stu-id="e2763-326">Use the `../me/onenote/` path instead.</span></span>

### <a name="20151"></a><span data-ttu-id="e2763-327">20151</span><span class="sxs-lookup"><span data-stu-id="e2763-327">20151</span></span>
<span data-ttu-id="e2763-328">Недопустимый запрос для этого типа проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e2763-328">The request is not valid for this authentication type.</span></span> <span data-ttu-id="e2763-329">Используйте конечную точку `../me/onenote/section/{id}/pages`, чтобы создать страницу в определенном разделе.</span><span class="sxs-lookup"><span data-stu-id="e2763-329">Use the `../me/onenote/section/{id}/pages` endpoint to create a page in a specific section.</span></span>

### <a name="20152"></a><span data-ttu-id="e2763-330">20152</span><span class="sxs-lookup"><span data-stu-id="e2763-330">20152 (EntityNameEmpty)</span></span>
<span data-ttu-id="e2763-p144">Не указано значение name для элемента. Имя должно быть определено, и оно не может содержать только пробелы.</span><span class="sxs-lookup"><span data-stu-id="e2763-p144">There is no name value specified for the entity. The name must be defined, and it cannot contain whitespaces only.</span></span>

### <a name="20153"></a><span data-ttu-id="e2763-333">20153</span><span class="sxs-lookup"><span data-stu-id="e2763-333">20153 (EntityNameInvalidChar)</span></span>
<span data-ttu-id="e2763-334">Имя объекта содержит недопустимые символы.</span><span class="sxs-lookup"><span data-stu-id="e2763-334">The entity name contains invalid characters.</span></span> <span data-ttu-id="e2763-335">Имя не может содержать следующие символы: `? * \ / : < > | & # " % ~`</span><span class="sxs-lookup"><span data-stu-id="e2763-335">The name cannot contain the following characters: `? * \ / : < > | & # " % ~`</span></span>

### <a name="20154"></a><span data-ttu-id="e2763-336">20154</span><span class="sxs-lookup"><span data-stu-id="e2763-336">20154 (EntityNameInvalidStart)</span></span>
<span data-ttu-id="e2763-337">Имя объекта не может начинаться с пробела.</span><span class="sxs-lookup"><span data-stu-id="e2763-337">The entity name cannot start with a space.</span></span>

### <a name="20155"></a><span data-ttu-id="e2763-338">20155</span><span class="sxs-lookup"><span data-stu-id="e2763-338">20155 (EntityNameTooLong)</span></span>
<span data-ttu-id="e2763-339">Слишком длинное имя объекта.</span><span class="sxs-lookup"><span data-stu-id="e2763-339">The entity name is too long.</span></span> <span data-ttu-id="e2763-340">Максимальная длина для имен записных книжек составляет 128 символов.</span><span class="sxs-lookup"><span data-stu-id="e2763-340">Notebook names have a 128-character limit.</span></span> <span data-ttu-id="e2763-341">Максимальная длина имен других объектов составляет 50 символов.</span><span class="sxs-lookup"><span data-stu-id="e2763-341">Other entity names have a 50-character limit.</span></span>

### <a name="20156"></a><span data-ttu-id="e2763-342">20156</span><span class="sxs-lookup"><span data-stu-id="e2763-342">20156</span></span>
<span data-ttu-id="e2763-343">Указанный идентификатор ресурса назначения не существует.</span><span class="sxs-lookup"><span data-stu-id="e2763-343">The specified ID for the destination resource does not exist.</span></span>

### <a name="20157"></a><span data-ttu-id="e2763-344">20157</span><span class="sxs-lookup"><span data-stu-id="e2763-344">20157</span></span>
<span data-ttu-id="e2763-345">Указан недопустимый идентификатор объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="e2763-345">The specified ID for the destination entity is invalid.</span></span>

### <a name="20158"></a><span data-ttu-id="e2763-346">20158</span><span class="sxs-lookup"><span data-stu-id="e2763-346">20158</span></span>
<span data-ttu-id="e2763-347">Не удалось получить метаданные для URL-адреса сайта, указанного в запросе.</span><span class="sxs-lookup"><span data-stu-id="e2763-347">Unable to get metadata for the site URL specified in the request.</span></span> <span data-ttu-id="e2763-348">Проверьте формат предоставленного URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="e2763-348">Check the format of the supplied URL.</span></span> <span data-ttu-id="e2763-349">К поддерживаемым форматам относятся `https://domain.sharepoint.com/site-a` и `https://domain.com/sites/site-a`.</span><span class="sxs-lookup"><span data-stu-id="e2763-349">Supported formats include `https://domain.sharepoint.com/site-a` and `https://domain.com/sites/site-a`.</span></span>

### <a name="20160"></a><span data-ttu-id="e2763-350">20160</span><span class="sxs-lookup"><span data-stu-id="e2763-350">20160</span></span>
<span data-ttu-id="e2763-351">Не удается найти единую группу Office 365 с указанным ИД.</span><span class="sxs-lookup"><span data-stu-id="e2763-351">Unable to find an Office 365 unified group that has the specified ID.</span></span>

### <a name="20161"></a><span data-ttu-id="e2763-352">20161</span><span class="sxs-lookup"><span data-stu-id="e2763-352">20161</span></span>
<span data-ttu-id="e2763-353">В контексте не указан действительный ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="e2763-353">The context does not specify a valid user ID.</span></span> <span data-ttu-id="e2763-354">Одна из распространенных ошибок — передача PUID/CID в виде значения типа long, а не hex.</span><span class="sxs-lookup"><span data-stu-id="e2763-354">One common error is that PUID/CID was passed in as a long instead of a hex.</span></span>

### <a name="20166"></a><span data-ttu-id="e2763-355">20166</span><span class="sxs-lookup"><span data-stu-id="e2763-355">20166</span></span>
<span data-ttu-id="e2763-356">Приложение отправило слишком много запросов от имени пользователя за короткий период времени.</span><span class="sxs-lookup"><span data-stu-id="e2763-356">The application has issued too many requests on behalf of a user in a short period of time.</span></span> <span data-ttu-id="e2763-357">Чтобы гарантировать стабильность и оперативность работы API OneNote, API возвращает код состояния 429 и это сообщение об ошибке, если обнаруживается, что приложение использует слишком много ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e2763-357">To help ensure that the OneNote API remains stable and responsive, the API returns a 429 status code and this error when it detects that an application is using too many resources.</span></span> 

<span data-ttu-id="e2763-358">Дополнительные сведения см. в статье [Регулирование API OneNote и как его избежать](https://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx).</span><span class="sxs-lookup"><span data-stu-id="e2763-358">For more information, see [OneNote API throttling and how to avoid it](https://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx).</span></span>

### <a name="20168"></a><span data-ttu-id="e2763-359">20168</span><span class="sxs-lookup"><span data-stu-id="e2763-359">20168</span></span>
<span data-ttu-id="e2763-360">Источник видео, указанный в запросе, не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2763-360">The video source specified in the request is not supported.</span></span> <span data-ttu-id="e2763-361">См. актуальный список [поддерживаемых сайтов с видео](onenote-images-files.md#adding-videos).</span><span class="sxs-lookup"><span data-stu-id="e2763-361">See [Supported video sites](onenote-images-files.md#adding-videos) for the current list.</span></span>


## <a name="codes-from-30001-to-39999"></a><span data-ttu-id="e2763-362">Коды от 30001 до 39999</span><span class="sxs-lookup"><span data-stu-id="e2763-362">Codes from 30001 to 39999</span></span>
<span data-ttu-id="e2763-363">Что-то не так с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="e2763-363">Something is wrong with the user's account.</span></span>

### <a name="30101"></a><span data-ttu-id="e2763-364">30101</span><span class="sxs-lookup"><span data-stu-id="e2763-364">30101</span></span>
<span data-ttu-id="e2763-365">Для учетной записи пользователя превышена квота OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e2763-365">The user account has exceeded its OneDrive quota.</span></span> <span data-ttu-id="e2763-366">См. страницу [OneDrive](https://onedrive.live.com/about/ru-RU/).</span><span class="sxs-lookup"><span data-stu-id="e2763-366">See [OneDrive](https://onedrive.live.com/about/ru-RU/).</span></span>

### <a name="30102"></a><span data-ttu-id="e2763-367">30102</span><span class="sxs-lookup"><span data-stu-id="e2763-367">30102</span></span>
<span data-ttu-id="e2763-368">В запрошенные раздел невозможно что-либо добавить, так как он достиг своего максимального размера.</span><span class="sxs-lookup"><span data-stu-id="e2763-368">Nothing more can be added to the requested section because it has reached its maximum size.</span></span>

### <a name="30103"></a><span data-ttu-id="e2763-369">30103</span><span class="sxs-lookup"><span data-stu-id="e2763-369">30103</span></span>
<span data-ttu-id="e2763-370">Для выполнения запроса используется слишком много ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e2763-370">Resource consumption is too high for the request.</span></span> <span data-ttu-id="e2763-371">Либо целевая учетная запись пользователя содержит слишком большой набор данных, либо служба получает слишком много одновременных запросов для одного сайта (например, личного сайта пользователя или сайта группы).</span><span class="sxs-lookup"><span data-stu-id="e2763-371">Either the target user account has a large dataset, or the service is receiving a high number of concurrent requests to the same site (for example, the user's personal site or a team site).</span></span>

### <a name="30104"></a><span data-ttu-id="e2763-372">30104</span><span class="sxs-lookup"><span data-stu-id="e2763-372">30104</span></span>
<span data-ttu-id="e2763-373">Работа учетной записи пользователя была приостановлена.</span><span class="sxs-lookup"><span data-stu-id="e2763-373">The user account has been suspended.</span></span>

### <a name="30105"></a><span data-ttu-id="e2763-374">30105</span><span class="sxs-lookup"><span data-stu-id="e2763-374">30105</span></span>
<span data-ttu-id="e2763-375">Личный сайт пользователя в OneDrive для бизнеса не подготовлен к работе. Это необходимо для доступа к записным книжкам.</span><span class="sxs-lookup"><span data-stu-id="e2763-375">The user's personal OneDrive for Business site is not provisioned, which is required to access notebooks.</span></span> <span data-ttu-id="e2763-376">Служба OneNote подготовит сайт к работе.</span><span class="sxs-lookup"><span data-stu-id="e2763-376">The OneNote service will provision the site now.</span></span> <span data-ttu-id="e2763-377">Этот процесс может занять несколько минут.</span><span class="sxs-lookup"><span data-stu-id="e2763-377">This process may take several minutes.</span></span>

### <a name="30106"></a><span data-ttu-id="e2763-378">30106</span><span class="sxs-lookup"><span data-stu-id="e2763-378">30106</span></span>
<span data-ttu-id="e2763-379">OneDrive для бизнеса подготавливается к работе для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e2763-379">OneDrive for Business is being provisioned for the user.</span></span>

### <a name="30108"></a><span data-ttu-id="e2763-380">30108</span><span class="sxs-lookup"><span data-stu-id="e2763-380">30108</span></span>
<span data-ttu-id="e2763-381">Не удалось получить личное хранилище пользователя в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e2763-381">The user's personal OneDrive for Business could not be retrieved.</span></span> <span data-ttu-id="e2763-382">В приведенной ниже таблице перечислены некоторые возможные причины.</span><span class="sxs-lookup"><span data-stu-id="e2763-382">The following table lists some possible causes.</span></span>

| <span data-ttu-id="e2763-383">Причина</span><span class="sxs-lookup"><span data-stu-id="e2763-383">Cause</span></span> | <span data-ttu-id="e2763-384">Решение</span><span class="sxs-lookup"><span data-stu-id="e2763-384">Resolution</span></span> |
|:------|:------|
| <span data-ttu-id="e2763-385">Личный сайт пользователя не подготовлен к работе.</span><span class="sxs-lookup"><span data-stu-id="e2763-385">The user's personal site has not been provisioned.</span></span> | <span data-ttu-id="e2763-386">Пользователь должен открыть OneDrive для бизнеса и следовать указаниям по подготовке сайта к работе.</span><span class="sxs-lookup"><span data-stu-id="e2763-386">The user should open OneDrive for Business and follow any instructions to provision the site.</span></span> <span data-ttu-id="e2763-387">Если проблема не будет устранена, необходимо обратиться к администратору клиента Office 365.</span><span class="sxs-lookup"><span data-stu-id="e2763-387">If this fails, they should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="e2763-388">В данный момент личный сайт пользователя подготавливается к работе.</span><span class="sxs-lookup"><span data-stu-id="e2763-388">The user's personal site is currently being provisioned.</span></span> | <span data-ttu-id="e2763-389">Попробуйте отправить запрос позже.</span><span class="sxs-lookup"><span data-stu-id="e2763-389">Try the request later.</span></span> |
| <span data-ttu-id="e2763-390">У пользователя нет действительной лицензии на OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e2763-390">The user does not have a valid OneDrive for Business license.</span></span> | <span data-ttu-id="e2763-391">Пользователь должен обратиться к администратору своего клиента Office 365.</span><span class="sxs-lookup"><span data-stu-id="e2763-391">The user should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="e2763-392">Не удается отправить запрос из-за проблем с сетью.</span><span class="sxs-lookup"><span data-stu-id="e2763-392">A network issue prevented the request from being successfully sent.</span></span> | <span data-ttu-id="e2763-393">Попробуйте отправить запрос позже.</span><span class="sxs-lookup"><span data-stu-id="e2763-393">Try the request later.</span></span> |

### <a name="30109"></a><span data-ttu-id="e2763-394">30109</span><span class="sxs-lookup"><span data-stu-id="e2763-394">30109</span></span>
<span data-ttu-id="e2763-395">Некоторые пользователи, указанные в запросе, не существуют.</span><span class="sxs-lookup"><span data-stu-id="e2763-395">Some users in the request do not exist.</span></span>

### <a name="30110"></a><span data-ttu-id="e2763-396">30110</span><span class="sxs-lookup"><span data-stu-id="e2763-396">30110</span></span>
<span data-ttu-id="e2763-397">Для этого клиента не зарегистрированы службы сведений об учащихся.</span><span class="sxs-lookup"><span data-stu-id="e2763-397">Student Information Services has not been registered for this tenant.</span></span>

### <a name="30111"></a><span data-ttu-id="e2763-398">30111</span><span class="sxs-lookup"><span data-stu-id="e2763-398">30111</span></span>
<span data-ttu-id="e2763-399">Возникла общая ошибка служб сведений об учащихся.</span><span class="sxs-lookup"><span data-stu-id="e2763-399">There is a generic error with Student Information Services.</span></span>

### <a name="30112"></a><span data-ttu-id="e2763-400">30112</span><span class="sxs-lookup"><span data-stu-id="e2763-400">30112</span></span>
<span data-ttu-id="e2763-401">Запрос влияет на нескольких пользователей с одинаковыми именами.</span><span class="sxs-lookup"><span data-stu-id="e2763-401">Multiple users affected by the request had the same username.</span></span>

### <a name="30113"></a><span data-ttu-id="e2763-402">30113</span><span class="sxs-lookup"><span data-stu-id="e2763-402">30113</span></span>
<span data-ttu-id="e2763-403">Для записной книжки не разрешены приглашения.</span><span class="sxs-lookup"><span data-stu-id="e2763-403">The notebook is not configured to allow invites.</span></span>

### <a name="30114"></a><span data-ttu-id="e2763-404">30114</span><span class="sxs-lookup"><span data-stu-id="e2763-404">30114</span></span>
<span data-ttu-id="e2763-405">Отсутствует обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e2763-405">There is a required parameter missing.</span></span>

## <a name="codes-from-40001-to-49999"></a><span data-ttu-id="e2763-406">Коды от 40001 до 49999</span><span class="sxs-lookup"><span data-stu-id="e2763-406">Codes from 40001 to 49999</span></span>
<span data-ttu-id="e2763-407">У пользователя или приложения нет необходимых разрешений.</span><span class="sxs-lookup"><span data-stu-id="e2763-407">The user or application does not have the correct permissions.</span></span>

### <a name="40001"></a><span data-ttu-id="e2763-408">40001</span><span class="sxs-lookup"><span data-stu-id="e2763-408">40001</span></span>
<span data-ttu-id="e2763-409">Запрос не содержит действительный маркер OAuth.</span><span class="sxs-lookup"><span data-stu-id="e2763-409">The request doesn't contain a valid OAuth token.</span></span> <span data-ttu-id="e2763-410">См. раздел [Разрешения для заметок](permissions-reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="e2763-410">See [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

### <a name="40002"></a><span data-ttu-id="e2763-411">40002</span><span class="sxs-lookup"><span data-stu-id="e2763-411">40002</span></span>
<span data-ttu-id="e2763-412">У пользователя нет разрешения на запись в указанном расположении.</span><span class="sxs-lookup"><span data-stu-id="e2763-412">The user doesn't have permission to write to the requested location.</span></span>

### <a name="40003"></a><span data-ttu-id="e2763-413">40003</span><span class="sxs-lookup"><span data-stu-id="e2763-413">40003</span></span>
<span data-ttu-id="e2763-414">У пользователя нет разрешения на доступ к запрашиваемому ресурсу.</span><span class="sxs-lookup"><span data-stu-id="e2763-414">The user doesn't have permission to access the requested resource.</span></span>

### <a name="40004"></a><span data-ttu-id="e2763-415">40004</span><span class="sxs-lookup"><span data-stu-id="e2763-415">40004</span></span>
<span data-ttu-id="e2763-416">Область действия маркера OAuth недостаточна для выполнения запрашиваемого действия.</span><span class="sxs-lookup"><span data-stu-id="e2763-416">The OAuth token doesn't have the required scopes to perform the requested action.</span></span> <span data-ttu-id="e2763-417">См. раздел [Разрешения для заметок](permissions-reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="e2763-417">See [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

### <a name="40006"></a><span data-ttu-id="e2763-418">40006</span><span class="sxs-lookup"><span data-stu-id="e2763-418">40006</span></span> 
<span data-ttu-id="e2763-419">Область действия маркера OAuth недостаточна для выполнения запрашиваемого действия.</span><span class="sxs-lookup"><span data-stu-id="e2763-419">The OAuth token doesn't have the required scopes to perform the requested action.</span></span> <span data-ttu-id="e2763-420">В частности, это относится к разрешению на редактирование.</span><span class="sxs-lookup"><span data-stu-id="e2763-420">Specifically the edit permission.</span></span> <span data-ttu-id="e2763-421">См. раздел [Разрешения для заметок](permissions-reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="e2763-421">See [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

### <a name="40007"></a><span data-ttu-id="e2763-422">40007</span><span class="sxs-lookup"><span data-stu-id="e2763-422">40007</span></span>
<span data-ttu-id="e2763-423">У пользователя нет разрешений на доступ к этому ресурсу.</span><span class="sxs-lookup"><span data-stu-id="e2763-423">The user does not have permissions to access this resource.</span></span>

### <a name="40008"></a><span data-ttu-id="e2763-424">40008</span><span class="sxs-lookup"><span data-stu-id="e2763-424">40008</span></span>
<span data-ttu-id="e2763-425">Доступ к этому ресурсу запрещен.</span><span class="sxs-lookup"><span data-stu-id="e2763-425">Access is Forbidden for this resource.</span></span>

### <a name="40009"></a><span data-ttu-id="e2763-426">40009</span><span class="sxs-lookup"><span data-stu-id="e2763-426">40009</span></span>
<span data-ttu-id="e2763-427">Контейнер уже используется другим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="e2763-427">The container is already in use by another resource.</span></span>

## <a name="see-also"></a><span data-ttu-id="e2763-428">См. также</span><span class="sxs-lookup"><span data-stu-id="e2763-428">See also</span></span>

- [<span data-ttu-id="e2763-429">Сообщения об ошибках и типы ресурсов ошибок Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e2763-429">Microsoft Graph error responses and resource types</span></span>](errors.md)
- [<span data-ttu-id="e2763-430">Справочник по OneNote</span><span class="sxs-lookup"><span data-stu-id="e2763-430">OneNote reference</span></span>](/graph/api/resources/onenote?view=graph-rest-1.0)

