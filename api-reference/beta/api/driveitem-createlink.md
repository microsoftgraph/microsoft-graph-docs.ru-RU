---
author: JeremyKelley
description: Используя действие createLink, вы можете поделиться ресурсом DriveItem с помощью ссылки для совместного доступа.
title: 'driveItem: createLink'
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a6f3c172efdec9decf2f054a8afbb8d7ccf53034
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941475"
---
# <a name="driveitem-createlink"></a><span data-ttu-id="2dc4f-103">driveItem: createLink</span><span class="sxs-lookup"><span data-stu-id="2dc4f-103">driveItem: createLink</span></span>

<span data-ttu-id="2dc4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dc4f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dc4f-105">Используя действие **createLink**, вы можете поделиться ресурсом [DriveItem](../resources/driveitem.md) с помощью ссылки для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-105">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="2dc4f-p101">Действие **createLink** создает ссылку для совместного доступа, если ссылка указанного типа еще не существует для приложения, совершающего вызов. Если для приложения уже создана такая ссылка указанного типа, возвращается она.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="2dc4f-108">Ресурсы DriveItem наследуют разрешения совместного доступа от своих предков.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-108">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="2dc4f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2dc4f-109">Permissions</span></span>

<span data-ttu-id="2dc4f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2dc4f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dc4f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2dc4f-112">Permission type</span></span>      | <span data-ttu-id="2dc4f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2dc4f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2dc4f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2dc4f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2dc4f-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dc4f-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2dc4f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2dc4f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2dc4f-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dc4f-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2dc4f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2dc4f-118">Application</span></span> | <span data-ttu-id="2dc4f-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dc4f-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2dc4f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2dc4f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```
## <a name="request-headers"></a><span data-ttu-id="2dc4f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2dc4f-121">Request headers</span></span>
|<span data-ttu-id="2dc4f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2dc4f-122">Name</span></span>|<span data-ttu-id="2dc4f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2dc4f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2dc4f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2dc4f-124">Authorization</span></span>|<span data-ttu-id="2dc4f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2dc4f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2dc4f-127">Content-Type</span></span>|<span data-ttu-id="2dc4f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dc4f-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2dc4f-130">Request body</span></span>

<span data-ttu-id="2dc4f-131">В теле запроса определяются свойства ссылки для совместного доступа, запрашиваемой приложением.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-131">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="2dc4f-132">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-132">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="2dc4f-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="2dc4f-133">Property</span></span>                 |  <span data-ttu-id="2dc4f-134">Тип</span><span class="sxs-lookup"><span data-stu-id="2dc4f-134">Type</span></span>  |                                 <span data-ttu-id="2dc4f-135">Описание</span><span class="sxs-lookup"><span data-stu-id="2dc4f-135">Description</span></span>                                                               |
| :----------------------| :----- | :---------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="2dc4f-136">type</span><span class="sxs-lookup"><span data-stu-id="2dc4f-136">type</span></span>|<span data-ttu-id="2dc4f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="2dc4f-137">String</span></span>|<span data-ttu-id="2dc4f-138">Optional.The type of sharing link to create.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-138">Optional.The type of sharing link to create.</span></span>   |
|<span data-ttu-id="2dc4f-139">scope</span><span class="sxs-lookup"><span data-stu-id="2dc4f-139">scope</span></span>|<span data-ttu-id="2dc4f-140">String</span><span class="sxs-lookup"><span data-stu-id="2dc4f-140">String</span></span>|<span data-ttu-id="2dc4f-141">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-141">Optional.</span></span> <span data-ttu-id="2dc4f-142">Область создаваемой ссылки.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-142">The scope of link to create.</span></span> <span data-ttu-id="2dc4f-143">Анонимные, организации или пользователи.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-143">Either anonymous, organization or users.</span></span>|
|<span data-ttu-id="2dc4f-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2dc4f-144">expirationDateTime</span></span>|<span data-ttu-id="2dc4f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dc4f-145">DateTimeOffset</span></span>|<span data-ttu-id="2dc4f-146">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-146">Optional.</span></span> <span data-ttu-id="2dc4f-147">Строка с форматом yyyy-MM-ddTHH:mm:ssZ dateTime указывает срок действия разрешения.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-147">A String with format of yyyy-MM-ddTHH:mm:ssZ of DateTime indicates the expiration time of the permission.</span></span>|
|<span data-ttu-id="2dc4f-148">password</span><span class="sxs-lookup"><span data-stu-id="2dc4f-148">password</span></span>|<span data-ttu-id="2dc4f-149">Строка</span><span class="sxs-lookup"><span data-stu-id="2dc4f-149">String</span></span>|<span data-ttu-id="2dc4f-150">Optional.The password of the sharing link that is set by the creator.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-150">Optional.The password of the sharing link that is set by the creator.</span></span>|
|<span data-ttu-id="2dc4f-151">recipients</span><span class="sxs-lookup"><span data-stu-id="2dc4f-151">recipients</span></span>|<span data-ttu-id="2dc4f-152">[коллекция driveRecipient](../resources/driverecipient.md)</span><span class="sxs-lookup"><span data-stu-id="2dc4f-152">[driveRecipient](../resources/driverecipient.md) collection</span></span>|<span data-ttu-id="2dc4f-153">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-153">Optional.</span></span> <span data-ttu-id="2dc4f-154">Коллекция получателей, которые получат доступ к ссылке общего доступа.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-154">A collection of recipients who will receive access to the sharing link.</span></span>|

### <a name="link-types"></a><span data-ttu-id="2dc4f-155">Типы ссылок</span><span class="sxs-lookup"><span data-stu-id="2dc4f-155">Link types</span></span>

<span data-ttu-id="2dc4f-156">Параметр **type** может принимать указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-156">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="2dc4f-157">Значение типа</span><span class="sxs-lookup"><span data-stu-id="2dc4f-157">Type value</span></span> | <span data-ttu-id="2dc4f-158">Описание</span><span class="sxs-lookup"><span data-stu-id="2dc4f-158">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| <span data-ttu-id="2dc4f-159">представление</span><span class="sxs-lookup"><span data-stu-id="2dc4f-159">view</span></span>           | <span data-ttu-id="2dc4f-160">Создает ссылку только для чтения на элемент.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-160">Creates a read-only link to the Item.</span></span>                                                                        |
| <span data-ttu-id="2dc4f-161">обзор</span><span class="sxs-lookup"><span data-stu-id="2dc4f-161">review</span></span>         | <span data-ttu-id="2dc4f-162">Создает ссылку на просмотр элемента.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-162">Creates a review link to the Item.</span></span> <span data-ttu-id="2dc4f-163">Этот параметр доступен только для файлов в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-163">This option is only available for files in OneDrive for Business and SharePoint.</span></span>                   |
| <span data-ttu-id="2dc4f-164">edit</span><span class="sxs-lookup"><span data-stu-id="2dc4f-164">edit</span></span>           | <span data-ttu-id="2dc4f-165">Создает ссылку для чтения на элемент.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-165">Creates an read-write link to the Item.</span></span>                                                                       |
| <span data-ttu-id="2dc4f-166">Внедрить</span><span class="sxs-lookup"><span data-stu-id="2dc4f-166">embed</span></span>          | <span data-ttu-id="2dc4f-167">Создает встраивную ссылку на элемент.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-167">Creates an embeddable link to the Item.</span></span>                                                                      |
| <span data-ttu-id="2dc4f-168">blocksDownload</span><span class="sxs-lookup"><span data-stu-id="2dc4f-168">blocksDownload</span></span> | <span data-ttu-id="2dc4f-169">Создает ссылку только для чтения, которая блокирует загрузку элемента.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-169">Creates a read-only link that blocks download to the Item.</span></span> <span data-ttu-id="2dc4f-170">Этот параметр доступен только для файлов в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-170">This option is only available for files in OneDrive for Business and SharePoint.</span></span>  |
| <span data-ttu-id="2dc4f-171">createOnly</span><span class="sxs-lookup"><span data-stu-id="2dc4f-171">createOnly</span></span>     | <span data-ttu-id="2dc4f-172">Создает ссылку на элемент только для загрузки.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-172">Creates an upload-only link to the Item.</span></span> <span data-ttu-id="2dc4f-173">Этот параметр доступен только для папок в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-173">This option is only available for folders in OneDrive for Business and SharePoint.</span></span>             |
| <span data-ttu-id="2dc4f-174">addressBar</span><span class="sxs-lookup"><span data-stu-id="2dc4f-174">addressBar</span></span>     | <span data-ttu-id="2dc4f-175">Создает ссылку по умолчанию, которая отображается в барах адресов браузера для вновь созданных файлов.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-175">Creates the default link that is shown in the browser address bars for newly created files.</span></span> <span data-ttu-id="2dc4f-176">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-176">Only available in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="2dc4f-177">Администратор организации настраивает, поддерживается ли этот тип ссылок и какие функции поддерживаются этим типом ссылок.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-177">The organization admin configures whether this link type is supported, and what features are supported by this link type.</span></span> |
| <span data-ttu-id="2dc4f-178">adminDefault</span><span class="sxs-lookup"><span data-stu-id="2dc4f-178">adminDefault</span></span>   | <span data-ttu-id="2dc4f-179">Создает по умолчанию ссылку на DriveItem, определяемую администратором организации.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-179">Creates the default link to the DriveItem as determined by the administrator of the organization.</span></span> <span data-ttu-id="2dc4f-180">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-180">Only available in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="2dc4f-181">Политика для организации выполняется администратором.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-181">The policy is enforced for the organization by the admin</span></span> |

### <a name="scope-types"></a><span data-ttu-id="2dc4f-182">Типы областей</span><span class="sxs-lookup"><span data-stu-id="2dc4f-182">Scope types</span></span>

<span data-ttu-id="2dc4f-183">Параметр **scope** может принимать указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-183">The following values are allowed for the **scope** parameter.</span></span>

| <span data-ttu-id="2dc4f-184">Значение</span><span class="sxs-lookup"><span data-stu-id="2dc4f-184">Value</span></span>          | <span data-ttu-id="2dc4f-185">Описание</span><span class="sxs-lookup"><span data-stu-id="2dc4f-185">Description</span></span>
|:---------------|:------------------------------------------------------------
| <span data-ttu-id="2dc4f-186">анонимный</span><span class="sxs-lookup"><span data-stu-id="2dc4f-186">anonymous</span></span>    | <span data-ttu-id="2dc4f-187">Любой пользователь со ссылкой обладает правом доступа без необходимости входа в систему.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-187">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="2dc4f-188">Это также относится к людям вне вашей организации.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-188">This may include people outside of your organization.</span></span> <span data-ttu-id="2dc4f-189">Администратор может отключить поддержку ссылок, не требующих проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-189">Anonymous link support may be disabled by an administrator.</span></span>
| <span data-ttu-id="2dc4f-190">organization;</span><span class="sxs-lookup"><span data-stu-id="2dc4f-190">organization</span></span> | <span data-ttu-id="2dc4f-191">Любой пользователь, вошедший в вашу организацию (клиент), может использовать ссылку для получения доступа.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-191">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="2dc4f-192">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-192">Only available in OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="2dc4f-193">users</span><span class="sxs-lookup"><span data-stu-id="2dc4f-193">users</span></span>        | <span data-ttu-id="2dc4f-194">Конкретные люди из коллекции получателей могут использовать ссылку для получения доступа.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-194">Specific people in the recipients collection can use the link to get access.</span></span> <span data-ttu-id="2dc4f-195">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-195">Only available in OneDrive for Business and SharePoint.</span></span>

## <a name="response"></a><span data-ttu-id="2dc4f-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="2dc4f-196">Response</span></span>

<span data-ttu-id="2dc4f-197">В случае успешного выполнения этот метод возвращает в тексте ответа один ресурс [Permission](../resources/permission.md), представляющий запрашиваемые разрешения для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-197">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="2dc4f-198">Если для элемента создается новая ссылка совместного доступа, возвращается код ответа `201 Created`, а если возвращается существующая ссылка — код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-198">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="examples"></a><span data-ttu-id="2dc4f-199">Примеры</span><span class="sxs-lookup"><span data-stu-id="2dc4f-199">Examples</span></span>

### <a name="example-1-create-an-anonymous-sharing-link"></a><span data-ttu-id="2dc4f-200">Пример 1. Создание анонимной ссылки на общий доступ</span><span class="sxs-lookup"><span data-stu-id="2dc4f-200">Example 1: Create an anonymous sharing link</span></span>
<span data-ttu-id="2dc4f-201">В приведенном ниже примере запрашивается создание ссылки для совместного доступа к объекту DriveItem, указанному по {itemId}, в хранилище OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-201">The following example requests a sharing link to be created for the DriveItem specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="2dc4f-202">Ссылка для совместного доступа подразумевает доступ только для чтения, и ее может использовать каждый, кому она предоставлена.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-202">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

#### <a name="request"></a><span data-ttu-id="2dc4f-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="2dc4f-203">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "driveItem_createlink",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-Type: application/json
Content-length: 212

{
  "type": "view",
  "scope": "anonymous",
  "password": "String",
  "recipients": [
    {
      "@odata.type": "microsoft.graph.driveRecipient"
    }
  ]
}
```

# <a name="c"></a>[<span data-ttu-id="2dc4f-204">C#</span><span class="sxs-lookup"><span data-stu-id="2dc4f-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-createlink-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2dc4f-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2dc4f-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-createlink-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2dc4f-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2dc4f-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-createlink-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2dc4f-207">Java</span><span class="sxs-lookup"><span data-stu-id="2dc4f-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/item-createlink-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2dc4f-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="2dc4f-208">Response</span></span>
><span data-ttu-id="2dc4f-209">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-209">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  },
  "hasPassword": true
}
```

### <a name="example-2-creating-company-sharable-links"></a><span data-ttu-id="2dc4f-210">Пример 2. Создание sharable ссылок компании</span><span class="sxs-lookup"><span data-stu-id="2dc4f-210">Example 2: Creating company sharable links</span></span>

<span data-ttu-id="2dc4f-211">OneDrive для бизнеса и SharePoint поддерживают ссылки с возможностью общего доступа в компании.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-211">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="2dc4f-212">Они аналогичны ссылкам, не требующим проверки подлинности, но работают только для элементов соответствующей организации.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-212">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="2dc4f-213">Чтобы создать такую ссылку, задайте для параметра **scope** значение `organization`.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-213">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

#### <a name="request"></a><span data-ttu-id="2dc4f-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="2dc4f-214">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create-link-scoped",
  "scopes": "files.readwrite service.sharepoint",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
 } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```
# <a name="c"></a>[<span data-ttu-id="2dc4f-215">C#</span><span class="sxs-lookup"><span data-stu-id="2dc4f-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-scoped-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2dc4f-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2dc4f-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-scoped-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2dc4f-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2dc4f-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-scoped-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2dc4f-218">Java</span><span class="sxs-lookup"><span data-stu-id="2dc4f-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-link-scoped-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2dc4f-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="2dc4f-219">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

### <a name="example-3-creating-embeddable-links"></a><span data-ttu-id="2dc4f-220">Пример 3. Создание встраивемых ссылок</span><span class="sxs-lookup"><span data-stu-id="2dc4f-220">Example 3: Creating embeddable links</span></span>

<span data-ttu-id="2dc4f-p119">При использовании типа ссылки `embed` возвращаемое значение webUrl можно внедрять в элемент HTML `<iframe>`. При создании встроенной ссылки свойство `webHtml` содержит HTML-код для объекта `<iframe>`, в котором размещается содержимое.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-p119">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

><span data-ttu-id="2dc4f-223">**Примечание.** Внедрение ссылок поддерживается только в личных учетных записях OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-223">**Note:** Embed links are only supported for OneDrive personal.</span></span>

#### <a name="request"></a><span data-ttu-id="2dc4f-224">Запросить</span><span class="sxs-lookup"><span data-stu-id="2dc4f-224">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create-embedded-link",
  "scopes": "files.readwrite service.onedrive",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
} -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```
# <a name="c"></a>[<span data-ttu-id="2dc4f-225">C#</span><span class="sxs-lookup"><span data-stu-id="2dc4f-225">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-embedded-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2dc4f-226">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2dc4f-226">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-embedded-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2dc4f-227">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2dc4f-227">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-embedded-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2dc4f-228">Java</span><span class="sxs-lookup"><span data-stu-id="2dc4f-228">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-embedded-link-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2dc4f-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="2dc4f-229">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["read"],
  "link": {
    "type": "embed",
    "webHtml": "<IFRAME src=\"https://onedrive.live.com/...\"></IFRAME>",
    "webUrl": "https://onedive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a><span data-ttu-id="2dc4f-230">Примечания</span><span class="sxs-lookup"><span data-stu-id="2dc4f-230">Remarks</span></span>

* <span data-ttu-id="2dc4f-231">Чтобы создать ссылку на основе политики по умолчанию организации и разрешений вызываемого в listItem, ограничьте параметры области и типа</span><span class="sxs-lookup"><span data-stu-id="2dc4f-231">To create a link based on the organization's default policy and the caller's permissions on the listItem, omit the scope and type parameters</span></span>
* <span data-ttu-id="2dc4f-232">Срок действия ссылок, созданных с помощью этого действия, не истекает при условии, что в организации не включена политика срока действия.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-232">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="2dc4f-233">Ссылки отображаются в разрешениях на совместное использование для элемента и могут быть удалены владельцем элемента.</span><span class="sxs-lookup"><span data-stu-id="2dc4f-233">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="2dc4f-234">Они всегда указывают на текущую версию элемента, если он не был извлечен (только в SharePoint).</span><span class="sxs-lookup"><span data-stu-id="2dc4f-234">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
}
-->