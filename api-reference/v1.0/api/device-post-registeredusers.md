---
title: Создание объекта registeredUser
description: Добавление зарегистрированного пользователя устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fddf0bffb3cd09caa7397fb29d111bc75e48e85c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002925"
---
# <a name="create-registereduser"></a><span data-ttu-id="aa35c-103">Создание объекта registeredUser</span><span class="sxs-lookup"><span data-stu-id="aa35c-103">Create registeredUser</span></span>

<span data-ttu-id="aa35c-104">Добавление зарегистрированного пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="aa35c-104">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa35c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa35c-105">Permissions</span></span>
<span data-ttu-id="aa35c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa35c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="aa35c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa35c-108">Permission type</span></span>      | <span data-ttu-id="aa35c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa35c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa35c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa35c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aa35c-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aa35c-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aa35c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa35c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa35c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa35c-113">Not supported.</span></span>    |
|<span data-ttu-id="aa35c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa35c-114">Application</span></span> | <span data-ttu-id="aa35c-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa35c-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa35c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa35c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="aa35c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa35c-117">Request headers</span></span>
| <span data-ttu-id="aa35c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="aa35c-118">Name</span></span>       | <span data-ttu-id="aa35c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="aa35c-119">Type</span></span> | <span data-ttu-id="aa35c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="aa35c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aa35c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa35c-121">Authorization</span></span>  | <span data-ttu-id="aa35c-122">string</span><span class="sxs-lookup"><span data-stu-id="aa35c-122">string</span></span>  | <span data-ttu-id="aa35c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa35c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa35c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aa35c-125">Request body</span></span>
<span data-ttu-id="aa35c-126">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa35c-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="aa35c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa35c-127">Response</span></span>

<span data-ttu-id="aa35c-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa35c-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa35c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="aa35c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa35c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa35c-130">Request</span></span>
<span data-ttu-id="aa35c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa35c-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="aa35c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa35c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aa35c-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="aa35c-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="aa35c-134">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa35c-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="aa35c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa35c-135">Response</span></span>
<span data-ttu-id="aa35c-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa35c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create registeredUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
