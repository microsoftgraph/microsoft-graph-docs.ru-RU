---
title: 'driveItem: Preview'
description: Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a49a05e1e01616bc9bbbb713fd05805d9af3070
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454372"
---
# <a name="driveitem-preview"></a><span data-ttu-id="5ed19-103">driveItem: Preview</span><span class="sxs-lookup"><span data-stu-id="5ed19-103">driveItem: preview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ed19-104">Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.</span><span class="sxs-lookup"><span data-stu-id="5ed19-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="5ed19-105">Если вы хотите получить ссылки с большим сроком действия, используйте вместо этого API [CreateLink][] .</span><span class="sxs-lookup"><span data-stu-id="5ed19-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="5ed19-106">**Примечание:** В настоящее время действие **Предварительный просмотр** доступно только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="5ed19-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="5ed19-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ed19-108">Permissions</span></span>

<span data-ttu-id="5ed19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ed19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ed19-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ed19-111">Permission type</span></span>                        | <span data-ttu-id="5ed19-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ed19-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="5ed19-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ed19-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ed19-114">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL, sites. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="5ed19-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="5ed19-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ed19-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ed19-116">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5ed19-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="5ed19-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ed19-117">Application</span></span>                            | <span data-ttu-id="5ed19-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ed19-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="5ed19-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ed19-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="5ed19-120">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ed19-120">Request body</span></span>

<span data-ttu-id="5ed19-121">В теле запроса определяются свойства внедряемого URL-адреса, запрашиваемого приложением.</span><span class="sxs-lookup"><span data-stu-id="5ed19-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="5ed19-122">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="5ed19-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="5ed19-123">Имя</span><span class="sxs-lookup"><span data-stu-id="5ed19-123">Name</span></span>      |  <span data-ttu-id="5ed19-124">Тип</span><span class="sxs-lookup"><span data-stu-id="5ed19-124">Type</span></span>         | <span data-ttu-id="5ed19-125">Описание</span><span class="sxs-lookup"><span data-stu-id="5ed19-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="5ed19-126">Просмотр</span><span class="sxs-lookup"><span data-stu-id="5ed19-126">viewer</span></span>      | <span data-ttu-id="5ed19-127">string</span><span class="sxs-lookup"><span data-stu-id="5ed19-127">string</span></span>        | <span data-ttu-id="5ed19-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="5ed19-128">Optional.</span></span> <span data-ttu-id="5ed19-129">Предварительная версия приложения для использования.</span><span class="sxs-lookup"><span data-stu-id="5ed19-129">Preview app to use.</span></span> <span data-ttu-id="5ed19-130">`onedrive` или `office`.</span><span class="sxs-lookup"><span data-stu-id="5ed19-130">`onedrive` or `office`.</span></span> <span data-ttu-id="5ed19-131">Если значение равно null, подходящее средство просмотра будет выбрано автоматически.</span><span class="sxs-lookup"><span data-stu-id="5ed19-131">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="5ed19-132">не для Chrome</span><span class="sxs-lookup"><span data-stu-id="5ed19-132">chromeless</span></span>  | <span data-ttu-id="5ed19-133">boolean</span><span class="sxs-lookup"><span data-stu-id="5ed19-133">boolean</span></span>       | <span data-ttu-id="5ed19-134">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5ed19-134">Optional.</span></span> <span data-ttu-id="5ed19-135">Если `true` выбрано значение (по умолчанию), то Внедренное представление не будет содержать элементы управления.</span><span class="sxs-lookup"><span data-stu-id="5ed19-135">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="5ed19-136">Алловедит</span><span class="sxs-lookup"><span data-stu-id="5ed19-136">allowEdit</span></span>   | <span data-ttu-id="5ed19-137">boolean</span><span class="sxs-lookup"><span data-stu-id="5ed19-137">boolean</span></span>       | <span data-ttu-id="5ed19-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5ed19-138">Optional.</span></span> <span data-ttu-id="5ed19-139">Если `true`файл можно редактировать из встроенного пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="5ed19-139">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="5ed19-140">page</span><span class="sxs-lookup"><span data-stu-id="5ed19-140">page</span></span>        | <span data-ttu-id="5ed19-141">строка или число</span><span class="sxs-lookup"><span data-stu-id="5ed19-141">string/number</span></span> | <span data-ttu-id="5ed19-142">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="5ed19-142">Optional.</span></span> <span data-ttu-id="5ed19-143">Номер страницы для начала документа, если это необходимо.</span><span class="sxs-lookup"><span data-stu-id="5ed19-143">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="5ed19-144">Указывается как строка для будущих случаев использования для типов файлов, таких как ZIP.</span><span class="sxs-lookup"><span data-stu-id="5ed19-144">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="5ed19-145">zoom</span><span class="sxs-lookup"><span data-stu-id="5ed19-145">zoom</span></span>        | <span data-ttu-id="5ed19-146">number</span><span class="sxs-lookup"><span data-stu-id="5ed19-146">number</span></span>        | <span data-ttu-id="5ed19-147">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="5ed19-147">Optional.</span></span> <span data-ttu-id="5ed19-148">Масштаб (при необходимости) для запуска.</span><span class="sxs-lookup"><span data-stu-id="5ed19-148">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="5ed19-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ed19-149">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="5ed19-150">Ответом будет объект JSON, содержащий следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="5ed19-150">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="5ed19-151">Имя</span><span class="sxs-lookup"><span data-stu-id="5ed19-151">Name</span></span>           | <span data-ttu-id="5ed19-152">Тип</span><span class="sxs-lookup"><span data-stu-id="5ed19-152">Type</span></span>   | <span data-ttu-id="5ed19-153">Описание</span><span class="sxs-lookup"><span data-stu-id="5ed19-153">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="5ed19-154">Команда</span><span class="sxs-lookup"><span data-stu-id="5ed19-154">getUrl</span></span>         | <span data-ttu-id="5ed19-155">строка</span><span class="sxs-lookup"><span data-stu-id="5ed19-155">string</span></span> | <span data-ttu-id="5ed19-156">URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)</span><span class="sxs-lookup"><span data-stu-id="5ed19-156">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="5ed19-157">Постурл</span><span class="sxs-lookup"><span data-stu-id="5ed19-157">postUrl</span></span>        | <span data-ttu-id="5ed19-158">строка</span><span class="sxs-lookup"><span data-stu-id="5ed19-158">string</span></span> | <span data-ttu-id="5ed19-159">URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)</span><span class="sxs-lookup"><span data-stu-id="5ed19-159">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="5ed19-160">Параметры</span><span class="sxs-lookup"><span data-stu-id="5ed19-160">postParameters</span></span> | <span data-ttu-id="5ed19-161">строка</span><span class="sxs-lookup"><span data-stu-id="5ed19-161">string</span></span> | <span data-ttu-id="5ed19-162">Параметры POST для включения при использовании Постурл</span><span class="sxs-lookup"><span data-stu-id="5ed19-162">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="5ed19-163">В зависимости от текущего состояния поддержки внедрения для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.</span><span class="sxs-lookup"><span data-stu-id="5ed19-163">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="5ed19-164">i-параметры — это строка, `application/x-www-form-urlencoded`отформатированная как, и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры.</span><span class="sxs-lookup"><span data-stu-id="5ed19-164">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="5ed19-165">Пример:</span><span class="sxs-lookup"><span data-stu-id="5ed19-165">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="5ed19-166">Наблюдател</span><span class="sxs-lookup"><span data-stu-id="5ed19-166">Viewers</span></span>

<span data-ttu-id="5ed19-167">Для параметра **средства просмотра** разрешены следующие значения.</span><span class="sxs-lookup"><span data-stu-id="5ed19-167">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="5ed19-168">Значение типа</span><span class="sxs-lookup"><span data-stu-id="5ed19-168">Type value</span></span> | <span data-ttu-id="5ed19-169">Описание</span><span class="sxs-lookup"><span data-stu-id="5ed19-169">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="5ed19-170">определен</span><span class="sxs-lookup"><span data-stu-id="5ed19-170">(null)</span></span>     | <span data-ttu-id="5ed19-171">Выбирает соответствующее приложение для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="5ed19-171">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="5ed19-172">В большинстве случаев будет использоваться `onedrive` предварительный просмотр, но он может варьироваться в зависимости от типа файла.</span><span class="sxs-lookup"><span data-stu-id="5ed19-172">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="5ed19-173">Использование приложения предварительного просмотра OneDrive для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="5ed19-173">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="5ed19-174">Используйте WAC (Office Online) для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="5ed19-174">Use the WAC (Office online) to render the file.</span></span> <span data-ttu-id="5ed19-175">Допускается только для документов Office.</span><span class="sxs-lookup"><span data-stu-id="5ed19-175">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="5ed19-176">Хром VS Chrome</span><span class="sxs-lookup"><span data-stu-id="5ed19-176">Chrome vs chromeless</span></span>

<span data-ttu-id="5ed19-177">Если `chromeless` этот параметр имеет значение true, предварительный просмотр будет иметь исходное представление файла.</span><span class="sxs-lookup"><span data-stu-id="5ed19-177">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="5ed19-178">В противном случае для взаимодействия с документом или представлением могут отображаться дополнительные панели инструментов и кнопки.</span><span class="sxs-lookup"><span data-stu-id="5ed19-178">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="5ed19-179">Просмотр и редактирование</span><span class="sxs-lookup"><span data-stu-id="5ed19-179">View/edit</span></span>

<span data-ttu-id="5ed19-180">Если `allowEdit` имеет значение true, документ можно изменить с помощью встроенной предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="5ed19-180">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="5ed19-181">Эта возможность может быть недоступна для предварительных версий приложений и типов файлов.</span><span class="sxs-lookup"><span data-stu-id="5ed19-181">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="5ed19-182">Страница/масштаб</span><span class="sxs-lookup"><span data-stu-id="5ed19-182">Page/zoom</span></span>

<span data-ttu-id="5ed19-183">Параметры `page` и `zoom` могут быть недоступны для всех предварительных версий приложений, но будут применены, если это приложение поддерживает приложение предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="5ed19-183">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-preview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
