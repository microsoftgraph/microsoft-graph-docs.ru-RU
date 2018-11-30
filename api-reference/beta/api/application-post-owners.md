---
title: Создание владельца
description: Используйте этот интерфейс API для создания нового владельца.
ms.openlocfilehash: fdfbaf31b954b7621b7c59fc61741c12644aaf4b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076327"
---
# <a name="create-owner"></a><span data-ttu-id="de09a-103">Создание владельца</span><span class="sxs-lookup"><span data-stu-id="de09a-103">Create owner</span></span>

> <span data-ttu-id="de09a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="de09a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de09a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de09a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de09a-106">Используйте этот интерфейс API для создания нового владельца.</span><span class="sxs-lookup"><span data-stu-id="de09a-106">Use this API to create a new owner.</span></span>
## <a name="permissions"></a><span data-ttu-id="de09a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de09a-107">Permissions</span></span>
<span data-ttu-id="de09a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de09a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de09a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de09a-110">Permission type</span></span>      | <span data-ttu-id="de09a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de09a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de09a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de09a-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="de09a-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="de09a-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="de09a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de09a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de09a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de09a-115">Not supported.</span></span>    |
|<span data-ttu-id="de09a-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="de09a-116">Application</span></span> | <span data-ttu-id="de09a-117">Application.ReadWrite.OwnedBy и Directory.Read.All, Application.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="de09a-117">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="de09a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de09a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners

```
## <a name="request-headers"></a><span data-ttu-id="de09a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de09a-119">Request headers</span></span>
| <span data-ttu-id="de09a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="de09a-120">Name</span></span>       | <span data-ttu-id="de09a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="de09a-121">Type</span></span> | <span data-ttu-id="de09a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="de09a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="de09a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de09a-123">Authorization</span></span>  | <span data-ttu-id="de09a-124">string</span><span class="sxs-lookup"><span data-stu-id="de09a-124">string</span></span>  | <span data-ttu-id="de09a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de09a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de09a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de09a-127">Request body</span></span>
<span data-ttu-id="de09a-128">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de09a-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="de09a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="de09a-129">Response</span></span>

<span data-ttu-id="de09a-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de09a-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de09a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="de09a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de09a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="de09a-132">Request</span></span>
<span data-ttu-id="de09a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de09a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/owners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="de09a-134">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de09a-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="de09a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="de09a-135">Response</span></span>
<span data-ttu-id="de09a-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="de09a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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