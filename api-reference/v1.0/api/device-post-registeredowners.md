---
title: Создание объекта registeredOwner
description: Добавление пользователя в качестве зарегистрированного владельца устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 69d702f7ca1cb119dd98a30436531ea9bd54a1ea
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656442"
---
# <a name="create-registeredowner"></a><span data-ttu-id="6f6e3-103">Создание объекта registeredOwner</span><span class="sxs-lookup"><span data-stu-id="6f6e3-103">Create registeredOwner</span></span>

<span data-ttu-id="6f6e3-104">Добавление пользователя в качестве зарегистрированного владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="6f6e3-104">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="6f6e3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f6e3-105">Permissions</span></span>
<span data-ttu-id="6f6e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f6e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6f6e3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f6e3-108">Permission type</span></span>      | <span data-ttu-id="6f6e3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f6e3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f6e3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f6e3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6f6e3-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6f6e3-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6f6e3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f6e3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f6e3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f6e3-113">Not supported.</span></span>    |
|<span data-ttu-id="6f6e3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f6e3-114">Application</span></span> | <span data-ttu-id="6f6e3-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f6e3-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f6e3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f6e3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="6f6e3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f6e3-117">Request headers</span></span>
| <span data-ttu-id="6f6e3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6f6e3-118">Name</span></span>       | <span data-ttu-id="6f6e3-119">Тип</span><span class="sxs-lookup"><span data-stu-id="6f6e3-119">Type</span></span> | <span data-ttu-id="6f6e3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6f6e3-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6f6e3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f6e3-121">Authorization</span></span>  | <span data-ttu-id="6f6e3-122">string</span><span class="sxs-lookup"><span data-stu-id="6f6e3-122">string</span></span>  | <span data-ttu-id="6f6e3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f6e3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f6e3-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f6e3-125">Request body</span></span>
<span data-ttu-id="6f6e3-126">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f6e3-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6f6e3-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f6e3-127">Response</span></span>

<span data-ttu-id="6f6e3-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f6e3-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f6e3-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6f6e3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f6e3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f6e3-130">Request</span></span>
<span data-ttu-id="6f6e3-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f6e3-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="6f6e3-132">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f6e3-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6f6e3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f6e3-133">Response</span></span>
<span data-ttu-id="6f6e3-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f6e3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6f6e3-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="6f6e3-137">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6f6e3-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="6f6e3-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_device-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/device-post-registeredowners.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
