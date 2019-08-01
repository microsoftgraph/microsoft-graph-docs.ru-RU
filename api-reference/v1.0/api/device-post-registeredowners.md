---
title: Создание объекта registeredOwner
description: Добавление пользователя в качестве зарегистрированного владельца устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f4155e822f8eed989c096f15b4e0767ce237cd79
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015672"
---
# <a name="create-registeredowner"></a><span data-ttu-id="f96a0-103">Создание объекта registeredOwner</span><span class="sxs-lookup"><span data-stu-id="f96a0-103">Create registeredOwner</span></span>

<span data-ttu-id="f96a0-104">Добавление пользователя в качестве зарегистрированного владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="f96a0-104">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="f96a0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f96a0-105">Permissions</span></span>
<span data-ttu-id="f96a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f96a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f96a0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f96a0-108">Permission type</span></span>      | <span data-ttu-id="f96a0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f96a0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f96a0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f96a0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f96a0-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f96a0-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f96a0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f96a0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f96a0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f96a0-113">Not supported.</span></span>    |
|<span data-ttu-id="f96a0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f96a0-114">Application</span></span> | <span data-ttu-id="f96a0-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f96a0-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f96a0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f96a0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="f96a0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f96a0-117">Request headers</span></span>
| <span data-ttu-id="f96a0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f96a0-118">Name</span></span>       | <span data-ttu-id="f96a0-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f96a0-119">Type</span></span> | <span data-ttu-id="f96a0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f96a0-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f96a0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f96a0-121">Authorization</span></span>  | <span data-ttu-id="f96a0-122">string</span><span class="sxs-lookup"><span data-stu-id="f96a0-122">string</span></span>  | <span data-ttu-id="f96a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f96a0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f96a0-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f96a0-125">Request body</span></span>
<span data-ttu-id="f96a0-126">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f96a0-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f96a0-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f96a0-127">Response</span></span>

<span data-ttu-id="f96a0-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f96a0-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f96a0-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f96a0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f96a0-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f96a0-130">Request</span></span>
<span data-ttu-id="f96a0-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f96a0-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f96a0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f96a0-132">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f96a0-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="f96a0-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f96a0-134">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f96a0-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f96a0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f96a0-135">Response</span></span>
<span data-ttu-id="f96a0-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f96a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
