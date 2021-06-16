---
title: 'listItem: createLink'
description: Создание ссылки для обмена listItem
author: learafa
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b0d490139763e619a151e3152868f98c1f1b96e4
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941583"
---
# <a name="listitem-createlink"></a><span data-ttu-id="31dc9-103">listItem: createLink</span><span class="sxs-lookup"><span data-stu-id="31dc9-103">listItem: createLink</span></span>

<span data-ttu-id="31dc9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31dc9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31dc9-105">Создайте ссылку общего доступа для [listItem.](../resources/listitem.md)</span><span class="sxs-lookup"><span data-stu-id="31dc9-105">Create a sharing link for a [listItem](../resources/listitem.md).</span></span>

<span data-ttu-id="31dc9-106">Действие **createLink** создает новую ссылку общего доступа, если указанный тип ссылки еще не существует для вызываемого приложения.</span><span class="sxs-lookup"><span data-stu-id="31dc9-106">The **createLink** action creates a new sharing link if the specified link type doesn't already exist for the calling application.</span></span>
<span data-ttu-id="31dc9-107">Если для приложения уже существует ссылка общего доступа указанного типа, это действие возвращает существующую ссылку общего доступа.</span><span class="sxs-lookup"><span data-stu-id="31dc9-107">If a sharing link of the specified type already exists for the app, this action will return the existing sharing link.</span></span>

<span data-ttu-id="31dc9-108">**ресурсы listItem** наследуют разрешения на совместное использование [из списка,](../resources/list.md) в который находится элемент.</span><span class="sxs-lookup"><span data-stu-id="31dc9-108">**listItem** resources inherit sharing permissions from the [list](../resources/list.md) the item resides in.</span></span>

## <a name="permissions"></a><span data-ttu-id="31dc9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31dc9-109">Permissions</span></span>
<span data-ttu-id="31dc9-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="31dc9-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="31dc9-111">Дополнительные дополнительные информации, в том числе о выборе разрешений, см. [в см. в .](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="31dc9-111">To learn more, including how to choose permissions, see [permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31dc9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31dc9-112">Permission type</span></span>|<span data-ttu-id="31dc9-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31dc9-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31dc9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31dc9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="31dc9-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31dc9-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="31dc9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31dc9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31dc9-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31dc9-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="31dc9-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31dc9-118">Application</span></span> | <span data-ttu-id="31dc9-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31dc9-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31dc9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31dc9-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}
-->
``` http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
```

## <a name="request-headers"></a><span data-ttu-id="31dc9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31dc9-121">Request headers</span></span>
|<span data-ttu-id="31dc9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="31dc9-122">Name</span></span>|<span data-ttu-id="31dc9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="31dc9-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="31dc9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31dc9-124">Authorization</span></span>|<span data-ttu-id="31dc9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31dc9-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="31dc9-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31dc9-127">Content-Type</span></span>|<span data-ttu-id="31dc9-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31dc9-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="31dc9-130">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="31dc9-130">Request body</span></span>
<span data-ttu-id="31dc9-131">В теле запроса укажи JSON представление параметров.</span><span class="sxs-lookup"><span data-stu-id="31dc9-131">In the request body, provide a JSON representation of the parameters.</span></span>

<span data-ttu-id="31dc9-132">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="31dc9-132">The following table shows the parameters that can be used with this action.</span></span>

|   <span data-ttu-id="31dc9-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="31dc9-133">Property</span></span>             |  <span data-ttu-id="31dc9-134">Тип</span><span class="sxs-lookup"><span data-stu-id="31dc9-134">Type</span></span>  |           <span data-ttu-id="31dc9-135">Описание</span><span class="sxs-lookup"><span data-stu-id="31dc9-135">Description</span></span>                        |
| :----------------------| :----- | :--------------------------------------------|
|<span data-ttu-id="31dc9-136">type</span><span class="sxs-lookup"><span data-stu-id="31dc9-136">type</span></span>|<span data-ttu-id="31dc9-137">Строка</span><span class="sxs-lookup"><span data-stu-id="31dc9-137">String</span></span>|<span data-ttu-id="31dc9-138">Тип создаваемой ссылки для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="31dc9-138">The type of sharing link to create.</span></span> <span data-ttu-id="31dc9-139">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="31dc9-139">Optional.</span></span> |
|<span data-ttu-id="31dc9-140">scope</span><span class="sxs-lookup"><span data-stu-id="31dc9-140">scope</span></span>|<span data-ttu-id="31dc9-141">String</span><span class="sxs-lookup"><span data-stu-id="31dc9-141">String</span></span>|<span data-ttu-id="31dc9-142">Область создаваемой ссылки.</span><span class="sxs-lookup"><span data-stu-id="31dc9-142">The scope of link to create.</span></span> <span data-ttu-id="31dc9-143">Либо `anonymous` , `organization` или `users` .</span><span class="sxs-lookup"><span data-stu-id="31dc9-143">Either `anonymous`, `organization` or `users`.</span></span> <span data-ttu-id="31dc9-144">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="31dc9-144">Optional.</span></span> |
|<span data-ttu-id="31dc9-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="31dc9-145">expirationDateTime</span></span>|<span data-ttu-id="31dc9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31dc9-146">DateTimeOffset</span></span>|<span data-ttu-id="31dc9-147">Строка с форматом yyyy-MM-ddTHH:mm:ssZ dateTime указывает срок действия разрешения.</span><span class="sxs-lookup"><span data-stu-id="31dc9-147">A string with format of yyyy-MM-ddTHH:mm:ssZ of DateTime indicates the expiration time of the permission.</span></span> <span data-ttu-id="31dc9-148">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="31dc9-148">Optional.</span></span> |
|<span data-ttu-id="31dc9-149">password</span><span class="sxs-lookup"><span data-stu-id="31dc9-149">password</span></span>|<span data-ttu-id="31dc9-150">Строка</span><span class="sxs-lookup"><span data-stu-id="31dc9-150">String</span></span>|<span data-ttu-id="31dc9-151">Пароль ссылки общего доступа, за устанавливаемой создателем.</span><span class="sxs-lookup"><span data-stu-id="31dc9-151">The password of the sharing link that is set by the creator.</span></span> <span data-ttu-id="31dc9-152">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="31dc9-152">Optional.</span></span> |
|<span data-ttu-id="31dc9-153">recipients</span><span class="sxs-lookup"><span data-stu-id="31dc9-153">recipients</span></span>|<span data-ttu-id="31dc9-154">[коллекция driveRecipient](../resources/driverecipient.md)</span><span class="sxs-lookup"><span data-stu-id="31dc9-154">[driveRecipient](../resources/driverecipient.md) collection</span></span>|<span data-ttu-id="31dc9-155">Коллекция получателей, которые получат доступ к ссылке общего доступа.</span><span class="sxs-lookup"><span data-stu-id="31dc9-155">A collection of recipients who will receive access to the sharing link.</span></span> <span data-ttu-id="31dc9-156">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="31dc9-156">Optional.</span></span> |

### <a name="link-types"></a><span data-ttu-id="31dc9-157">Типы ссылок</span><span class="sxs-lookup"><span data-stu-id="31dc9-157">Link types</span></span>

<span data-ttu-id="31dc9-158">Параметр **type** может принимать указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="31dc9-158">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="31dc9-159">Значение типа</span><span class="sxs-lookup"><span data-stu-id="31dc9-159">Type value</span></span> | <span data-ttu-id="31dc9-160">Описание</span><span class="sxs-lookup"><span data-stu-id="31dc9-160">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| <span data-ttu-id="31dc9-161">представление</span><span class="sxs-lookup"><span data-stu-id="31dc9-161">view</span></span>           | <span data-ttu-id="31dc9-162">Создает ссылку на элемент, предполагающую доступ только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31dc9-162">Creates a read-only link to the item.</span></span>                                                                        |
| <span data-ttu-id="31dc9-163">обзор</span><span class="sxs-lookup"><span data-stu-id="31dc9-163">review</span></span>         | <span data-ttu-id="31dc9-164">Создает ссылку на обзор элемента.</span><span class="sxs-lookup"><span data-stu-id="31dc9-164">Creates a review link to the item.</span></span> <span data-ttu-id="31dc9-165">Этот параметр доступен только для файлов в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="31dc9-165">This option is only available for files in OneDrive for Business and SharePoint.</span></span>                   |
| <span data-ttu-id="31dc9-166">edit</span><span class="sxs-lookup"><span data-stu-id="31dc9-166">edit</span></span>           | <span data-ttu-id="31dc9-167">Создает ссылку на элемент для чтения.</span><span class="sxs-lookup"><span data-stu-id="31dc9-167">Creates an read-write link to the item.</span></span>                                                                       |
| <span data-ttu-id="31dc9-168">Внедрить</span><span class="sxs-lookup"><span data-stu-id="31dc9-168">embed</span></span>          | <span data-ttu-id="31dc9-169">Создает встроенную ссылку на элемент.</span><span class="sxs-lookup"><span data-stu-id="31dc9-169">Creates an embeddable link to the item.</span></span>                                                                      |
| <span data-ttu-id="31dc9-170">blocksDownload</span><span class="sxs-lookup"><span data-stu-id="31dc9-170">blocksDownload</span></span> | <span data-ttu-id="31dc9-171">Создает ссылку только для чтения, которая блокирует загрузку элемента.</span><span class="sxs-lookup"><span data-stu-id="31dc9-171">Creates a read-only link that blocks download to the item.</span></span> <span data-ttu-id="31dc9-172">Этот параметр доступен только для файлов в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="31dc9-172">This option is only available for files in OneDrive for Business and SharePoint.</span></span>  |
| <span data-ttu-id="31dc9-173">createOnly</span><span class="sxs-lookup"><span data-stu-id="31dc9-173">createOnly</span></span>     | <span data-ttu-id="31dc9-174">Создает ссылку на элемент только для загрузки.</span><span class="sxs-lookup"><span data-stu-id="31dc9-174">Creates an upload-only link to the item.</span></span> <span data-ttu-id="31dc9-175">Этот параметр доступен только для папок в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="31dc9-175">This option is only available for folders in OneDrive for Business and SharePoint.</span></span>             |
| <span data-ttu-id="31dc9-176">addressBar</span><span class="sxs-lookup"><span data-stu-id="31dc9-176">addressBar</span></span>     | <span data-ttu-id="31dc9-177">Создает ссылку по умолчанию, которая отображается в барах адресов браузера для вновь созданных файлов.</span><span class="sxs-lookup"><span data-stu-id="31dc9-177">Creates the default link that is shown in the browser address bars for newly created files.</span></span> <span data-ttu-id="31dc9-178">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="31dc9-178">Only available in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="31dc9-179">Администратор организации настраивает, поддерживается ли этот тип ссылок и какие функции поддерживаются этим типом ссылок.</span><span class="sxs-lookup"><span data-stu-id="31dc9-179">The organization admin configures whether this link type is supported, and what features are supported by this link type.</span></span> |
| <span data-ttu-id="31dc9-180">adminDefault</span><span class="sxs-lookup"><span data-stu-id="31dc9-180">adminDefault</span></span>   | <span data-ttu-id="31dc9-181">Создает ссылку по умолчанию на элемент, определяемую администратором организации.</span><span class="sxs-lookup"><span data-stu-id="31dc9-181">Creates the default link to the item as determined by the administrator of the organization.</span></span> <span data-ttu-id="31dc9-182">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="31dc9-182">Only available in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="31dc9-183">Политика для организации выполняется администратором.</span><span class="sxs-lookup"><span data-stu-id="31dc9-183">The policy is enforced for the organization by the admin</span></span> |

### <a name="scope-types"></a><span data-ttu-id="31dc9-184">Типы областей</span><span class="sxs-lookup"><span data-stu-id="31dc9-184">Scope types</span></span>

<span data-ttu-id="31dc9-185">Параметр **scope** может принимать указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="31dc9-185">The following values are allowed for the **scope** parameter.</span></span>

| <span data-ttu-id="31dc9-186">Значение</span><span class="sxs-lookup"><span data-stu-id="31dc9-186">Value</span></span>          | <span data-ttu-id="31dc9-187">Описание</span><span class="sxs-lookup"><span data-stu-id="31dc9-187">Description</span></span>
|:---------------|:------------------------------------------------------------
| <span data-ttu-id="31dc9-188">анонимный</span><span class="sxs-lookup"><span data-stu-id="31dc9-188">anonymous</span></span>    | <span data-ttu-id="31dc9-189">Любой пользователь со ссылкой обладает правом доступа без необходимости входа в систему.</span><span class="sxs-lookup"><span data-stu-id="31dc9-189">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="31dc9-190">Это также относится к людям вне вашей организации.</span><span class="sxs-lookup"><span data-stu-id="31dc9-190">This may include people outside of your organization.</span></span> <span data-ttu-id="31dc9-191">Администратор может отключить поддержку ссылок, не требующих проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="31dc9-191">Anonymous link support may be disabled by an administrator.</span></span>
| <span data-ttu-id="31dc9-192">organization;</span><span class="sxs-lookup"><span data-stu-id="31dc9-192">organization</span></span> | <span data-ttu-id="31dc9-193">Любой пользователь, вошедший в вашу организацию (клиент), может использовать ссылку для получения доступа.</span><span class="sxs-lookup"><span data-stu-id="31dc9-193">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="31dc9-194">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="31dc9-194">Only available in OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="31dc9-195">users</span><span class="sxs-lookup"><span data-stu-id="31dc9-195">users</span></span>        | <span data-ttu-id="31dc9-196">Конкретные люди из коллекции получателей могут использовать ссылку для получения доступа.</span><span class="sxs-lookup"><span data-stu-id="31dc9-196">Specific people in the recipients collection can use the link to get access.</span></span> <span data-ttu-id="31dc9-197">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="31dc9-197">Only available in OneDrive for Business and SharePoint.</span></span>

## <a name="response"></a><span data-ttu-id="31dc9-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="31dc9-198">Response</span></span>

<span data-ttu-id="31dc9-199">В случае успешного использования [](../resources/permission.md) этот метод возвращает один ресурс разрешений в органе отклика, который представляет запрашиваемую для обмена разрешениями.</span><span class="sxs-lookup"><span data-stu-id="31dc9-199">If successful, this method returns a single [permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="31dc9-200">Ответ будет, если для listItem создается новая ссылка общего доступа или возвращается `201 Created` `200 OK` существующая ссылка.</span><span class="sxs-lookup"><span data-stu-id="31dc9-200">The response will be `201 Created` if a new sharing link is created for the listItem or `200 OK` if an existing link is returned.</span></span>

## <a name="examples"></a><span data-ttu-id="31dc9-201">Примеры</span><span class="sxs-lookup"><span data-stu-id="31dc9-201">Examples</span></span>

### <a name="example-1-create-an-anonymous-sharing-link"></a><span data-ttu-id="31dc9-202">Пример 1. Создание анонимной ссылки на общий доступ</span><span class="sxs-lookup"><span data-stu-id="31dc9-202">Example 1: Create an anonymous sharing link</span></span>
<span data-ttu-id="31dc9-203">В следующем примере запрашивается ссылка общего доступа, которая будет создана для listItem, указанного {itemId} в указанном списке {listId}.</span><span class="sxs-lookup"><span data-stu-id="31dc9-203">The following example requests a sharing link to be created for the listItem specified by {itemId} in the list specified {listId}.</span></span>
<span data-ttu-id="31dc9-204">Ссылка для совместного доступа подразумевает доступ только для чтения, и ее может использовать каждый, кому она предоставлена.</span><span class="sxs-lookup"><span data-stu-id="31dc9-204">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

#### <a name="request"></a><span data-ttu-id="31dc9-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="31dc9-205">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST sites/{siteId}/lists/{listId}/items/{itemId}/createLink
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

#### <a name="response"></a><span data-ttu-id="31dc9-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="31dc9-206">Response</span></span>
><span data-ttu-id="31dc9-207">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="31dc9-207">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
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

### <a name="example-2-creating-company-sharable-links"></a><span data-ttu-id="31dc9-208">Пример 2. Создание sharable ссылок компании</span><span class="sxs-lookup"><span data-stu-id="31dc9-208">Example 2: Creating company sharable links</span></span>

<span data-ttu-id="31dc9-209">OneDrive для бизнеса и SharePoint поддерживают ссылки с возможностью общего доступа в компании.</span><span class="sxs-lookup"><span data-stu-id="31dc9-209">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="31dc9-210">Они аналогичны ссылкам, не требующим проверки подлинности, но работают только для элементов соответствующей организации.</span><span class="sxs-lookup"><span data-stu-id="31dc9-210">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="31dc9-211">Чтобы создать такую ссылку, задайте для параметра **scope** значение `organization`.</span><span class="sxs-lookup"><span data-stu-id="31dc9-211">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

#### <a name="request"></a><span data-ttu-id="31dc9-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="31dc9-212">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

#### <a name="response"></a><span data-ttu-id="31dc9-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="31dc9-213">Response</span></span>

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

### <a name="example-3-creating-embeddable-links"></a><span data-ttu-id="31dc9-214">Пример 3. Создание встраивемых ссылок</span><span class="sxs-lookup"><span data-stu-id="31dc9-214">Example 3: Creating embeddable links</span></span>

<span data-ttu-id="31dc9-p120">При использовании типа ссылки `embed` возвращаемое значение webUrl можно внедрять в элемент HTML `<iframe>`. При создании встроенной ссылки свойство `webHtml` содержит HTML-код для объекта `<iframe>`, в котором размещается содержимое.</span><span class="sxs-lookup"><span data-stu-id="31dc9-p120">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

><span data-ttu-id="31dc9-217">**Примечание.** Внедрение ссылок поддерживается только в личных учетных записях OneDrive.</span><span class="sxs-lookup"><span data-stu-id="31dc9-217">**Note:** Embed links are only supported for OneDrive personal.</span></span>

#### <a name="request"></a><span data-ttu-id="31dc9-218">Запросить</span><span class="sxs-lookup"><span data-stu-id="31dc9-218">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

#### <a name="response"></a><span data-ttu-id="31dc9-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="31dc9-219">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="31dc9-220">Примечания</span><span class="sxs-lookup"><span data-stu-id="31dc9-220">Remarks</span></span>

* <span data-ttu-id="31dc9-221">Чтобы создать ссылку на основе политики по умолчанию организации и разрешений вызываемого в listItem, ограничьте параметры области и типа</span><span class="sxs-lookup"><span data-stu-id="31dc9-221">To create a link based on the organization's default policy and the caller's permissions on the listItem, omit the scope and type parameters</span></span>
* <span data-ttu-id="31dc9-222">Срок действия ссылок, созданных с помощью этого действия, не истекает при условии, что в организации не включена политика срока действия.</span><span class="sxs-lookup"><span data-stu-id="31dc9-222">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="31dc9-223">Ссылки видны в разрешениях общего доступа для listItem и могут быть удалены владельцем listItem.</span><span class="sxs-lookup"><span data-stu-id="31dc9-223">Links are visible in the sharing permissions for the listItem and can be removed by an owner of the listItem.</span></span>
* <span data-ttu-id="31dc9-224">Ссылки всегда указывают на текущую версию listItem, если только listItem не будет SharePoint).</span><span class="sxs-lookup"><span data-stu-id="31dc9-224">Links always point to the current version of a listItem unless the listItem is checked out (SharePoint only).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for an listItem.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
}
-->