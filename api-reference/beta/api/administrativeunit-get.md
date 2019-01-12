---
title: Получение administrativeUnit
description: Извлечение свойств и связи объекта administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d91db6fa5365d9e0db7f655ecab75fa594b4ea8b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931946"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="a853a-103">Получение administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="a853a-103">Get administrativeUnit</span></span>

> <span data-ttu-id="a853a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a853a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a853a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a853a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a853a-106">Извлечение свойств и связи объекта [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="a853a-106">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="a853a-107">Поскольку ресурсов **administrativeUnit** поддерживает [расширения](/graph/extensibility-overview), вы также можете использовать `GET` операции для получения данных расширения и настраиваемых свойств в экземпляре **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="a853a-107">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="a853a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a853a-108">Permissions</span></span>
<span data-ttu-id="a853a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a853a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a853a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a853a-111">Permission type</span></span>      | <span data-ttu-id="a853a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a853a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a853a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a853a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a853a-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a853a-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a853a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a853a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a853a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a853a-116">Not supported.</span></span>    |
|<span data-ttu-id="a853a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a853a-117">Application</span></span> | <span data-ttu-id="a853a-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a853a-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a853a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a853a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a853a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a853a-120">Optional query parameters</span></span>
<span data-ttu-id="a853a-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a853a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a853a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a853a-122">Request headers</span></span>
| <span data-ttu-id="a853a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a853a-123">Name</span></span>      |<span data-ttu-id="a853a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a853a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a853a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a853a-125">Authorization</span></span>  | <span data-ttu-id="a853a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a853a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a853a-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a853a-128">Request body</span></span>
<span data-ttu-id="a853a-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a853a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a853a-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a853a-130">Response</span></span>

<span data-ttu-id="a853a-131">Успешно завершена, этот метод возвращает `200 OK` объект [administrativeUnit](../resources/administrativeunit.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a853a-131">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a853a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a853a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a853a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a853a-133">Request</span></span>
<span data-ttu-id="a853a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a853a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="a853a-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="a853a-135">Response</span></span>
<span data-ttu-id="a853a-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a853a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

## <a name="see-also"></a><span data-ttu-id="a853a-139">См. также</span><span class="sxs-lookup"><span data-stu-id="a853a-139">See also</span></span>

- [<span data-ttu-id="a853a-140">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="a853a-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a853a-141">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="a853a-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
