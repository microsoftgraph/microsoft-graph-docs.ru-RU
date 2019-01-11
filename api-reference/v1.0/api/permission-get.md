---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Получение разрешений
localization_priority: Normal
ms.openlocfilehash: 4d893724af2c695597f0d81d5ceb0649c30ad7b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864136"
---
# <a name="get-sharing-permission-for-a-file-or-folder"></a><span data-ttu-id="eaf0c-102">Получение разрешения на общий доступ для файла или папки</span><span class="sxs-lookup"><span data-stu-id="eaf0c-102">Get sharing permission for a file or folder</span></span>

<span data-ttu-id="eaf0c-103">В этой статье рассказывается, как возвратить действующее разрешение на общий доступ для конкретного ресурса разрешения.</span><span class="sxs-lookup"><span data-stu-id="eaf0c-103">Return the effective sharing permission for a particular permission resource.</span></span>

<span data-ttu-id="eaf0c-104">Действующие разрешения для элемента могут быть заданы непосредственно для элемента или унаследованы от его предков.</span><span class="sxs-lookup"><span data-stu-id="eaf0c-104">Effective permissions of an item can come from two sources: permissions set directly on the item itself or permissions that are inherited from the item's ancestors.</span></span>

<span data-ttu-id="eaf0c-p101">Вызывающая сторона может распознать унаследованное разрешение, проверив свойство `inheritedFrom`. Это свойство представляет собой ресурс [itemReference](../resources/itemreference.md), ссылающийся на элемент, от которого унаследовано разрешение.</span><span class="sxs-lookup"><span data-stu-id="eaf0c-p101">Callers can differentiate if the permission is inherited or not by checking the `inheritedFrom` property. This property is an [ItemReference](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="eaf0c-107">Уровни разрешений SharePoint, заданные для элемента, возвращаются с префиксом SP.</span><span class="sxs-lookup"><span data-stu-id="eaf0c-107">SharePoint permission levels set on an item are returned with an 'SP' prefix.</span></span> <span data-ttu-id="eaf0c-108">Примеры: SP.View Only, SP.Limited Access, SP.View Web Analytics Data.</span><span class="sxs-lookup"><span data-stu-id="eaf0c-108">For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data.</span></span> <span data-ttu-id="eaf0c-109">См. [полный список ролей SharePoint](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span><span class="sxs-lookup"><span data-stu-id="eaf0c-109">See [Full list of SharePoint roles](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span></span>

## <a name="permissions"></a><span data-ttu-id="eaf0c-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eaf0c-110">Permissions</span></span>

<span data-ttu-id="eaf0c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaf0c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaf0c-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eaf0c-113">Permission type</span></span>      | <span data-ttu-id="eaf0c-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eaf0c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eaf0c-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eaf0c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="eaf0c-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaf0c-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="eaf0c-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eaf0c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaf0c-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaf0c-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="eaf0c-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eaf0c-119">Application</span></span> | <span data-ttu-id="eaf0c-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaf0c-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eaf0c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eaf0c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
GET /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eaf0c-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eaf0c-122">Optional query parameters</span></span>

<span data-ttu-id="eaf0c-123">Этот метод поддерживает [параметр запроса $select](/graph/query-parameters) для формирования отклика.</span><span class="sxs-lookup"><span data-stu-id="eaf0c-123">This method support the [$select query parameter](/graph/query-parameters) to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="eaf0c-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="eaf0c-124">Response</span></span>

<span data-ttu-id="eaf0c-125">В случае успеха этот метод возвращает код отклика `200 OK` и ресурс [Permission](../resources/permission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eaf0c-125">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaf0c-126">Пример</span><span class="sxs-lookup"><span data-stu-id="eaf0c-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="eaf0c-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="eaf0c-127">Request</span></span>

<span data-ttu-id="eaf0c-128">Ниже показан пример запроса на доступ к разрешению для папки.</span><span class="sxs-lookup"><span data-stu-id="eaf0c-128">Here is an example of the request to access a permission on a folder.</span></span>

<!-- { "blockType": "request", "name": "get-item-permission", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a><span data-ttu-id="eaf0c-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="eaf0c-129">Response</span></span>

<span data-ttu-id="eaf0c-130">При успешном выполнении этот метод возвращает ресурс [Permission](../resources/permission.md) для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="eaf0c-130">If successful, this method returns a [Permission](../resources/permission.md) resource for the specified ID.</span></span> 

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```

## <a name="remarks"></a><span data-ttu-id="eaf0c-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="eaf0c-131">Remarks</span></span>

<span data-ttu-id="eaf0c-132">Ресурс [Permission](../resources/permission.md) использует _аспекты_ для предоставления сведений о типе разрешения, представленного ресурсом.</span><span class="sxs-lookup"><span data-stu-id="eaf0c-132">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="eaf0c-p104">Разрешения с аспектом [**link**](../resources/sharinglink.md) представляют ссылки для предоставления общего доступа, созданные для элемента. Такие ссылки содержат уникальный токен, предоставляющий доступ к элементу для любого пользователя, воспользовавшегося ссылкой.</span><span class="sxs-lookup"><span data-stu-id="eaf0c-p104">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="eaf0c-135">Разрешения с аспектом [**invitation**](../resources/sharinginvitation.md) представляют разрешения, добавленные при приглашении определенных пользователей или групп поработать с файлом.</span><span class="sxs-lookup"><span data-stu-id="eaf0c-135">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

### <a name="error-responses"></a><span data-ttu-id="eaf0c-136">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="eaf0c-136">Error responses</span></span>

<span data-ttu-id="eaf0c-137">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="eaf0c-137">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get a DriveItem's sharing permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions"
} -->
