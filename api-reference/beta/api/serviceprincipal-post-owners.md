---
title: 'servicePrincipal: Добавление владельца'
description: Используйте этот API, чтобы добавить владельца для субъекта-службы.
localization_priority: Normal
ms.openlocfilehash: 67146ddf8fc4705b7c55487ec868a5bb090ecfa7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537496"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="3df70-103">servicePrincipal: Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="3df70-103">servicePrincipal: Add owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3df70-104">Используйте этот API, чтобы добавить владельца для субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="3df70-104">Use this API to add an owner for the service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="3df70-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3df70-105">Permissions</span></span>
<span data-ttu-id="3df70-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3df70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3df70-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3df70-108">Permission type</span></span>      | <span data-ttu-id="3df70-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3df70-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3df70-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3df70-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3df70-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3df70-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3df70-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3df70-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3df70-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3df70-113">Not supported.</span></span>    |
|<span data-ttu-id="3df70-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3df70-114">Application</span></span> | <span data-ttu-id="3df70-115">Application. ReadWrite. Овнедби и Directory. Read. ALL, Application. ReadWrite. ALL и Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="3df70-115">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3df70-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3df70-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners

```
## <a name="request-headers"></a><span data-ttu-id="3df70-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3df70-117">Request headers</span></span>
| <span data-ttu-id="3df70-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3df70-118">Name</span></span>       | <span data-ttu-id="3df70-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3df70-119">Type</span></span> | <span data-ttu-id="3df70-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3df70-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3df70-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3df70-121">Authorization</span></span>  | <span data-ttu-id="3df70-122">string</span><span class="sxs-lookup"><span data-stu-id="3df70-122">string</span></span>  | <span data-ttu-id="3df70-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3df70-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3df70-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3df70-125">Request body</span></span>
<span data-ttu-id="3df70-126">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3df70-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3df70-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3df70-127">Response</span></span>

<span data-ttu-id="3df70-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3df70-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3df70-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3df70-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3df70-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3df70-130">Request</span></span>
<span data-ttu-id="3df70-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3df70-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/owners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="3df70-132">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3df70-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3df70-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3df70-133">Response</span></span>
<span data-ttu-id="3df70-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3df70-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-post-owners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
