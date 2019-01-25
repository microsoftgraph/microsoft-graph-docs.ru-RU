---
title: Обновите параметр каталога
description: Обновление свойства объекта параметр конкретного каталога.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: baaf6994f7052155173dd58b2c6b021939dc7ba7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529098"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="15fa0-103">Обновите параметр каталога</span><span class="sxs-lookup"><span data-stu-id="15fa0-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15fa0-104">Обновление свойства объекта параметр конкретного каталога.</span><span class="sxs-lookup"><span data-stu-id="15fa0-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="15fa0-105">**Примечание**: версия /beta этот интерфейс API является только относится к группам.</span><span class="sxs-lookup"><span data-stu-id="15fa0-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="15fa0-106">Для *обновления groupSettings*переименован версии /v1.0 этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="15fa0-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="15fa0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15fa0-107">Permissions</span></span>
<span data-ttu-id="15fa0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15fa0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15fa0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15fa0-110">Permission type</span></span>      | <span data-ttu-id="15fa0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15fa0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15fa0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15fa0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15fa0-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="15fa0-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="15fa0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15fa0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15fa0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15fa0-115">Not supported.</span></span>    |
|<span data-ttu-id="15fa0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15fa0-116">Application</span></span> | <span data-ttu-id="15fa0-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15fa0-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15fa0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15fa0-118">HTTP request</span></span>
<span data-ttu-id="15fa0-119"><!-- { "blockType": "ignored" } -->Обновление клиента всей или группу параметров.</span><span class="sxs-lookup"><span data-stu-id="15fa0-119"><!-- { "blockType": "ignored" } --> Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="15fa0-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15fa0-120">Optional request headers</span></span>
| <span data-ttu-id="15fa0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="15fa0-121">Name</span></span>       | <span data-ttu-id="15fa0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="15fa0-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="15fa0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15fa0-123">Authorization</span></span>  | <span data-ttu-id="15fa0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15fa0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="15fa0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15fa0-126">Request body</span></span>
<span data-ttu-id="15fa0-127">В теле запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="15fa0-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="15fa0-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="15fa0-128">Property</span></span>     | <span data-ttu-id="15fa0-129">Тип</span><span class="sxs-lookup"><span data-stu-id="15fa0-129">Type</span></span>   |<span data-ttu-id="15fa0-130">Описание</span><span class="sxs-lookup"><span data-stu-id="15fa0-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="15fa0-131">values</span><span class="sxs-lookup"><span data-stu-id="15fa0-131">values</span></span> | <span data-ttu-id="15fa0-132">settingValue</span><span class="sxs-lookup"><span data-stu-id="15fa0-132">settingValue</span></span> | <span data-ttu-id="15fa0-p104">Обновленный набор значений.  ПРИМЕЧАНИЕ. Необходимо предоставить весь набор коллекции. Вы не можете обновить отдельный набор значений.</span><span class="sxs-lookup"><span data-stu-id="15fa0-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="15fa0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="15fa0-136">Response</span></span>

<span data-ttu-id="15fa0-137">В случае успешного выполнения этот метод возвращает код отклика `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="15fa0-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="15fa0-138">Пример</span><span class="sxs-lookup"><span data-stu-id="15fa0-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15fa0-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="15fa0-139">Request</span></span>
<span data-ttu-id="15fa0-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15fa0-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_directorysetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/settings/{id}
Content-type: application/json
Content-length: 178

{
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="15fa0-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="15fa0-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update directorysetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
