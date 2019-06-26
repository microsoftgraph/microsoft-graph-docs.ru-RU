---
title: 'driveItem: Preview'
description: Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5e260e3dc360464b39daa5dde671a1bc11c9c6b6
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236302"
---
# <a name="driveitem-preview"></a><span data-ttu-id="d477e-103">driveItem: Preview</span><span class="sxs-lookup"><span data-stu-id="d477e-103">driveItem: preview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d477e-104">Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.</span><span class="sxs-lookup"><span data-stu-id="d477e-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="d477e-105">Если вы хотите получить ссылки с большим сроком действия, используйте вместо этого API [CreateLink][] .</span><span class="sxs-lookup"><span data-stu-id="d477e-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="d477e-106">**Примечание:** В настоящее время действие **Предварительный просмотр** доступно только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d477e-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="d477e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d477e-108">Permissions</span></span>

<span data-ttu-id="d477e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d477e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d477e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d477e-111">Permission type</span></span>                        | <span data-ttu-id="d477e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d477e-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="d477e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d477e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d477e-114">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL, sites. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="d477e-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="d477e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d477e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d477e-116">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d477e-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="d477e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d477e-117">Application</span></span>                            | <span data-ttu-id="d477e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d477e-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="d477e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d477e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="d477e-120">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d477e-120">Request body</span></span>

<span data-ttu-id="d477e-121">В теле запроса определяются свойства внедряемого URL-адреса, запрашиваемого приложением.</span><span class="sxs-lookup"><span data-stu-id="d477e-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="d477e-122">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="d477e-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="d477e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d477e-123">Name</span></span>      |  <span data-ttu-id="d477e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="d477e-124">Type</span></span>         | <span data-ttu-id="d477e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d477e-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="d477e-126">Просмотр</span><span class="sxs-lookup"><span data-stu-id="d477e-126">viewer</span></span>      | <span data-ttu-id="d477e-127">string</span><span class="sxs-lookup"><span data-stu-id="d477e-127">string</span></span>        | <span data-ttu-id="d477e-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d477e-128">Optional.</span></span> <span data-ttu-id="d477e-129">Предварительная версия приложения для использования.</span><span class="sxs-lookup"><span data-stu-id="d477e-129">Preview app to use.</span></span> <span data-ttu-id="d477e-130">`onedrive` или `office`.</span><span class="sxs-lookup"><span data-stu-id="d477e-130">`onedrive` or `office`.</span></span> <span data-ttu-id="d477e-131">Если значение равно null, подходящее средство просмотра будет выбрано автоматически.</span><span class="sxs-lookup"><span data-stu-id="d477e-131">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="d477e-132">не для Chrome</span><span class="sxs-lookup"><span data-stu-id="d477e-132">chromeless</span></span>  | <span data-ttu-id="d477e-133">boolean</span><span class="sxs-lookup"><span data-stu-id="d477e-133">boolean</span></span>       | <span data-ttu-id="d477e-134">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d477e-134">Optional.</span></span> <span data-ttu-id="d477e-135">Если `true` выбрано значение (по умолчанию), то Внедренное представление не будет содержать элементы управления.</span><span class="sxs-lookup"><span data-stu-id="d477e-135">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="d477e-136">Алловедит</span><span class="sxs-lookup"><span data-stu-id="d477e-136">allowEdit</span></span>   | <span data-ttu-id="d477e-137">boolean</span><span class="sxs-lookup"><span data-stu-id="d477e-137">boolean</span></span>       | <span data-ttu-id="d477e-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d477e-138">Optional.</span></span> <span data-ttu-id="d477e-139">Если `true`файл можно редактировать из встроенного пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="d477e-139">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="d477e-140">page</span><span class="sxs-lookup"><span data-stu-id="d477e-140">page</span></span>        | <span data-ttu-id="d477e-141">строка или число</span><span class="sxs-lookup"><span data-stu-id="d477e-141">string/number</span></span> | <span data-ttu-id="d477e-142">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d477e-142">Optional.</span></span> <span data-ttu-id="d477e-143">Номер страницы для начала документа, если это необходимо.</span><span class="sxs-lookup"><span data-stu-id="d477e-143">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="d477e-144">Указывается как строка для будущих случаев использования для типов файлов, таких как ZIP.</span><span class="sxs-lookup"><span data-stu-id="d477e-144">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="d477e-145">zoom</span><span class="sxs-lookup"><span data-stu-id="d477e-145">zoom</span></span>        | <span data-ttu-id="d477e-146">number</span><span class="sxs-lookup"><span data-stu-id="d477e-146">number</span></span>        | <span data-ttu-id="d477e-147">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d477e-147">Optional.</span></span> <span data-ttu-id="d477e-148">Масштаб (при необходимости) для запуска.</span><span class="sxs-lookup"><span data-stu-id="d477e-148">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="d477e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d477e-149">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="d477e-150">Ответом будет объект JSON, содержащий следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="d477e-150">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="d477e-151">Имя</span><span class="sxs-lookup"><span data-stu-id="d477e-151">Name</span></span>           | <span data-ttu-id="d477e-152">Тип</span><span class="sxs-lookup"><span data-stu-id="d477e-152">Type</span></span>   | <span data-ttu-id="d477e-153">Описание</span><span class="sxs-lookup"><span data-stu-id="d477e-153">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="d477e-154">Команда</span><span class="sxs-lookup"><span data-stu-id="d477e-154">getUrl</span></span>         | <span data-ttu-id="d477e-155">string</span><span class="sxs-lookup"><span data-stu-id="d477e-155">string</span></span> | <span data-ttu-id="d477e-156">URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)</span><span class="sxs-lookup"><span data-stu-id="d477e-156">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="d477e-157">Постурл</span><span class="sxs-lookup"><span data-stu-id="d477e-157">postUrl</span></span>        | <span data-ttu-id="d477e-158">string</span><span class="sxs-lookup"><span data-stu-id="d477e-158">string</span></span> | <span data-ttu-id="d477e-159">URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)</span><span class="sxs-lookup"><span data-stu-id="d477e-159">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="d477e-160">Параметры</span><span class="sxs-lookup"><span data-stu-id="d477e-160">postParameters</span></span> | <span data-ttu-id="d477e-161">string</span><span class="sxs-lookup"><span data-stu-id="d477e-161">string</span></span> | <span data-ttu-id="d477e-162">Параметры POST для включения при использовании Постурл</span><span class="sxs-lookup"><span data-stu-id="d477e-162">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="d477e-163">В зависимости от текущего состояния поддержки внедрения для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.</span><span class="sxs-lookup"><span data-stu-id="d477e-163">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="d477e-164">i-параметры — это строка, `application/x-www-form-urlencoded`отформатированная как, и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры.</span><span class="sxs-lookup"><span data-stu-id="d477e-164">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="d477e-165">Пример:</span><span class="sxs-lookup"><span data-stu-id="d477e-165">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="d477e-166">Наблюдател</span><span class="sxs-lookup"><span data-stu-id="d477e-166">Viewers</span></span>

<span data-ttu-id="d477e-167">Для параметра **средства просмотра** разрешены следующие значения.</span><span class="sxs-lookup"><span data-stu-id="d477e-167">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="d477e-168">Значение типа</span><span class="sxs-lookup"><span data-stu-id="d477e-168">Type value</span></span> | <span data-ttu-id="d477e-169">Описание</span><span class="sxs-lookup"><span data-stu-id="d477e-169">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="d477e-170">определен</span><span class="sxs-lookup"><span data-stu-id="d477e-170">(null)</span></span>     | <span data-ttu-id="d477e-171">Выбирает соответствующее приложение для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="d477e-171">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="d477e-172">В большинстве случаев будет использоваться `onedrive` предварительный просмотр, но он может варьироваться в зависимости от типа файла.</span><span class="sxs-lookup"><span data-stu-id="d477e-172">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="d477e-173">Использование приложения предварительного просмотра OneDrive для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="d477e-173">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="d477e-174">Используйте веб-версию Office для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="d477e-174">Use the web version of Office to render the file.</span></span> <span data-ttu-id="d477e-175">Допускается только для документов Office.</span><span class="sxs-lookup"><span data-stu-id="d477e-175">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="d477e-176">Хром VS Chrome</span><span class="sxs-lookup"><span data-stu-id="d477e-176">Chrome vs chromeless</span></span>

<span data-ttu-id="d477e-177">Если `chromeless` этот параметр имеет значение true, предварительный просмотр будет иметь исходное представление файла.</span><span class="sxs-lookup"><span data-stu-id="d477e-177">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="d477e-178">В противном случае для взаимодействия с документом или представлением могут отображаться дополнительные панели инструментов и кнопки.</span><span class="sxs-lookup"><span data-stu-id="d477e-178">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="d477e-179">Просмотр и редактирование</span><span class="sxs-lookup"><span data-stu-id="d477e-179">View/edit</span></span>

<span data-ttu-id="d477e-180">Если `allowEdit` имеет значение true, документ можно изменить с помощью встроенной предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="d477e-180">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="d477e-181">Эта возможность может быть недоступна для предварительных версий приложений и типов файлов.</span><span class="sxs-lookup"><span data-stu-id="d477e-181">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="d477e-182">Страница/масштаб</span><span class="sxs-lookup"><span data-stu-id="d477e-182">Page/zoom</span></span>

<span data-ttu-id="d477e-183">Параметры `page` и `zoom` могут быть недоступны для всех предварительных версий приложений, но будут применены, если это приложение поддерживает приложение предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="d477e-183">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
