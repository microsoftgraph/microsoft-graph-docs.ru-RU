---
title: Создание administrativeUnit
description: Используйте этот интерфейс API для создания нового administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 9ec6d1579e1a27317bd7d4e126a73a1b4175ec86
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859873"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="817f5-103">Создание administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="817f5-103">Create administrativeUnit</span></span>

> <span data-ttu-id="817f5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="817f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="817f5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="817f5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="817f5-106">Используйте этот интерфейс API для создания нового [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="817f5-106">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="817f5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="817f5-107">Permissions</span></span>
<span data-ttu-id="817f5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="817f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="817f5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="817f5-110">Permission type</span></span>      | <span data-ttu-id="817f5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="817f5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="817f5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="817f5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="817f5-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="817f5-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="817f5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="817f5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="817f5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="817f5-115">Not supported.</span></span>    |
|<span data-ttu-id="817f5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="817f5-116">Application</span></span> | <span data-ttu-id="817f5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="817f5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="817f5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="817f5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="817f5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="817f5-119">Request headers</span></span>
| <span data-ttu-id="817f5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="817f5-120">Name</span></span>      |<span data-ttu-id="817f5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="817f5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="817f5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="817f5-122">Authorization</span></span>  | <span data-ttu-id="817f5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="817f5-p103">Bearer {token}. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="817f5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="817f5-125">Request body</span></span>
<span data-ttu-id="817f5-126">В тексте запроса укажите представление JSON объекта [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="817f5-126">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="817f5-127">Поскольку ресурсов **administrativeUnit** поддерживает [расширения](/graph/extensibility-overview), можно использовать `POST` операции и Добавление настраиваемых свойств с собственными данными в административных единицу при его создании.</span><span class="sxs-lookup"><span data-stu-id="817f5-127">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="817f5-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="817f5-128">Response</span></span>

<span data-ttu-id="817f5-129">Успешно завершена, этот метод возвращает `201 Created` объект [administrativeUnit](../resources/administrativeunit.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="817f5-129">If successful, this method returns `201 Created` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="817f5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="817f5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="817f5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="817f5-131">Request</span></span>
<span data-ttu-id="817f5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="817f5-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="817f5-133">В тексте запроса укажите представление JSON объекта [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="817f5-133">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="817f5-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="817f5-134">Response</span></span>
<span data-ttu-id="817f5-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="817f5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="817f5-138">См. также</span><span class="sxs-lookup"><span data-stu-id="817f5-138">See also</span></span>

- [<span data-ttu-id="817f5-139">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="817f5-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="817f5-140">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="817f5-140">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
