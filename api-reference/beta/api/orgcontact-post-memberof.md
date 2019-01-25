---
title: Создание член групп
description: Используйте этот интерфейс API для создания нового член групп.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 466074d2d23dc4b991c8c153252028587fd5afcc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518921"
---
# <a name="create-memberof"></a><span data-ttu-id="cae78-103">Создание член групп</span><span class="sxs-lookup"><span data-stu-id="cae78-103">Create memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cae78-104">Используйте этот интерфейс API для создания нового член групп.</span><span class="sxs-lookup"><span data-stu-id="cae78-104">Use this API to create a new memberOf.</span></span>
## <a name="permissions"></a><span data-ttu-id="cae78-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cae78-105">Permissions</span></span>
<span data-ttu-id="cae78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cae78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cae78-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cae78-108">Permission type</span></span>      | <span data-ttu-id="cae78-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cae78-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cae78-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cae78-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cae78-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae78-111">Not supported.</span></span>    |
|<span data-ttu-id="cae78-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cae78-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cae78-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae78-113">Not supported.</span></span>    |
|<span data-ttu-id="cae78-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cae78-114">Application</span></span> | <span data-ttu-id="cae78-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae78-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cae78-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cae78-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="cae78-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cae78-117">Request headers</span></span>
| <span data-ttu-id="cae78-118">Имя</span><span class="sxs-lookup"><span data-stu-id="cae78-118">Name</span></span>       | <span data-ttu-id="cae78-119">Тип</span><span class="sxs-lookup"><span data-stu-id="cae78-119">Type</span></span> | <span data-ttu-id="cae78-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cae78-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cae78-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cae78-121">Authorization</span></span>  | <span data-ttu-id="cae78-122">string</span><span class="sxs-lookup"><span data-stu-id="cae78-122">string</span></span>  | <span data-ttu-id="cae78-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cae78-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cae78-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cae78-125">Request body</span></span>
<span data-ttu-id="cae78-126">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cae78-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cae78-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae78-127">Response</span></span>

<span data-ttu-id="cae78-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cae78-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cae78-129">Пример</span><span class="sxs-lookup"><span data-stu-id="cae78-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cae78-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="cae78-130">Request</span></span>
<span data-ttu-id="cae78-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cae78-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/memberOf
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="cae78-132">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cae78-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cae78-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="cae78-133">Response</span></span>
<span data-ttu-id="cae78-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cae78-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-post-memberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
