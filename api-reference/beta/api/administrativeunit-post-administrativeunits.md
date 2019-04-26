---
title: Создание administrativeUnit
description: Используйте этот API для создания нового administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4ed0eaf3d7d0618d41f218365840857a27b781c6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322784"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="d6f6d-103">Создание administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="d6f6d-103">Create administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6f6d-104">Используйте этот API для создания нового [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="d6f6d-104">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d6f6d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6f6d-105">Permissions</span></span>
<span data-ttu-id="d6f6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6f6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d6f6d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6f6d-108">Permission type</span></span>      | <span data-ttu-id="d6f6d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6f6d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6f6d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6f6d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d6f6d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d6f6d-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d6f6d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6f6d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6f6d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6f6d-113">Not supported.</span></span>    |
|<span data-ttu-id="d6f6d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6f6d-114">Application</span></span> | <span data-ttu-id="d6f6d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6f6d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6f6d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6f6d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="d6f6d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6f6d-117">Request headers</span></span>
| <span data-ttu-id="d6f6d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d6f6d-118">Name</span></span>      |<span data-ttu-id="d6f6d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d6f6d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d6f6d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6f6d-120">Authorization</span></span>  | <span data-ttu-id="d6f6d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6f6d-p102">Bearer {token}. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="d6f6d-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d6f6d-123">Request body</span></span>
<span data-ttu-id="d6f6d-124">В тексте запроса добавьте представление объекта [AdministrativeUnit](../resources/administrativeunit.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6f6d-124">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="d6f6d-125">Так как ресурс **administrativeUnit** поддерживает [расширения](/graph/extensibility-overview), вы можете использовать `POST` операцию и добавлять настраиваемые свойства с собственными данными в административную единицу при создании.</span><span class="sxs-lookup"><span data-stu-id="d6f6d-125">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="d6f6d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6f6d-126">Response</span></span>

<span data-ttu-id="d6f6d-127">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [administrativeUnit](../resources/administrativeunit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6f6d-127">If successful, this method returns `201 Created` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6f6d-128">Пример</span><span class="sxs-lookup"><span data-stu-id="d6f6d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6f6d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6f6d-129">Request</span></span>
<span data-ttu-id="d6f6d-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6f6d-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}-->
```http
POST https://graph.microsoft.com/beta/administrativeUnits
Content-type: application/json
Content-length: 150

{
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "true"
}
```
<span data-ttu-id="d6f6d-131">В тексте запроса добавьте представление объекта [AdministrativeUnit](../resources/administrativeunit.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6f6d-131">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d6f6d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6f6d-132">Response</span></span>
<span data-ttu-id="d6f6d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d6f6d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 172

{
  "administrativeUnit": {
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "true",
    "id": "7a3dc8f3-b3a0-4164-9a99-ed36f3af039f"
  }
}
```

## <a name="see-also"></a><span data-ttu-id="d6f6d-136">См. также</span><span class="sxs-lookup"><span data-stu-id="d6f6d-136">See also</span></span>

- [<span data-ttu-id="d6f6d-137">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="d6f6d-137">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d6f6d-138">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="d6f6d-138">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
