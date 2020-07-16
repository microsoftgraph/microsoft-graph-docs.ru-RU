---
title: Создание объекта registeredUser
description: Добавление зарегистрированного пользователя устройства.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 68b03be62fd05e787422f743c5ed2c31d8cb95f5
ms.sourcegitcommit: 9c1abb1c87177da20e1f5bbf1fae8131ab7e4f16
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146675"
---
# <a name="create-registereduser"></a><span data-ttu-id="7f4cb-103">Создание объекта registeredUser</span><span class="sxs-lookup"><span data-stu-id="7f4cb-103">Create registeredUser</span></span>

<span data-ttu-id="7f4cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f4cb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7f4cb-105">Добавление зарегистрированного пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="7f4cb-105">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f4cb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f4cb-106">Permissions</span></span>
<span data-ttu-id="7f4cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f4cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7f4cb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f4cb-109">Permission type</span></span>      | <span data-ttu-id="7f4cb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f4cb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f4cb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f4cb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7f4cb-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7f4cb-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7f4cb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f4cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f4cb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f4cb-114">Not supported.</span></span>    |
|<span data-ttu-id="7f4cb-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7f4cb-115">Application</span></span> | <span data-ttu-id="7f4cb-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4cb-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f4cb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f4cb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="7f4cb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f4cb-118">Request headers</span></span>
| <span data-ttu-id="7f4cb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7f4cb-119">Name</span></span>       | <span data-ttu-id="7f4cb-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7f4cb-120">Type</span></span> | <span data-ttu-id="7f4cb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7f4cb-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7f4cb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f4cb-122">Authorization</span></span>  | <span data-ttu-id="7f4cb-123">string</span><span class="sxs-lookup"><span data-stu-id="7f4cb-123">string</span></span>  | <span data-ttu-id="7f4cb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f4cb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f4cb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f4cb-126">Request body</span></span>
<span data-ttu-id="7f4cb-127">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f4cb-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7f4cb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f4cb-128">Response</span></span>

<span data-ttu-id="7f4cb-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7f4cb-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7f4cb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7f4cb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f4cb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f4cb-131">Request</span></span>
<span data-ttu-id="7f4cb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f4cb-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f4cb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f4cb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="7f4cb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f4cb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="7f4cb-135">C#</span><span class="sxs-lookup"><span data-stu-id="7f4cb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7f4cb-136">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f4cb-136">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7f4cb-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f4cb-137">Response</span></span>
<span data-ttu-id="7f4cb-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f4cb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No content
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
