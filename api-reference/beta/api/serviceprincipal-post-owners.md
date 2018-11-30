---
title: 'servicePrincipal: Добавление владельца'
description: Используйте этот интерфейс API для добавления владельца для участников-служб.
ms.openlocfilehash: 79ffb0d8d6c680b517421455cee011b3764c8f15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081018"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="0777c-103">servicePrincipal: Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="0777c-103">servicePrincipal: Add owner</span></span>

> <span data-ttu-id="0777c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0777c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0777c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0777c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0777c-106">Используйте этот интерфейс API для добавления владельца для участников-служб.</span><span class="sxs-lookup"><span data-stu-id="0777c-106">Use this API to add an owner for the service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="0777c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0777c-107">Permissions</span></span>
<span data-ttu-id="0777c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0777c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0777c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0777c-110">Permission type</span></span>      | <span data-ttu-id="0777c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0777c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0777c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0777c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0777c-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0777c-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0777c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0777c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0777c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0777c-115">Not supported.</span></span>    |
|<span data-ttu-id="0777c-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="0777c-116">Application</span></span> | <span data-ttu-id="0777c-117">Application.ReadWrite.OwnedBy и Directory.Read.All, Application.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0777c-117">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0777c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0777c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners

```
## <a name="request-headers"></a><span data-ttu-id="0777c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0777c-119">Request headers</span></span>
| <span data-ttu-id="0777c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0777c-120">Name</span></span>       | <span data-ttu-id="0777c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0777c-121">Type</span></span> | <span data-ttu-id="0777c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0777c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0777c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0777c-123">Authorization</span></span>  | <span data-ttu-id="0777c-124">string</span><span class="sxs-lookup"><span data-stu-id="0777c-124">string</span></span>  | <span data-ttu-id="0777c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0777c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0777c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0777c-127">Request body</span></span>
<span data-ttu-id="0777c-128">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0777c-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0777c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0777c-129">Response</span></span>

<span data-ttu-id="0777c-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0777c-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0777c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0777c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0777c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0777c-132">Request</span></span>
<span data-ttu-id="0777c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0777c-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="0777c-134">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0777c-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0777c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0777c-135">Response</span></span>
<span data-ttu-id="0777c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0777c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->