---
title: Перечисление educationClasses
description: Получите список объектов educationClass и их свойств.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6b599217cfb87a853fdc6630f210bea969cbaa97
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232258"
---
# <a name="list-educationclasses"></a><span data-ttu-id="cb770-103">Перечисление educationClasses</span><span class="sxs-lookup"><span data-stu-id="cb770-103">List educationClasses</span></span>

<span data-ttu-id="cb770-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb770-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb770-105">Получите список объектов [educationClass](../resources/educationclass.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="cb770-105">Get a list of the [educationClass](../resources/educationclass.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb770-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb770-106">Permissions</span></span>

<span data-ttu-id="cb770-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb770-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb770-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb770-109">Permission type</span></span>                        | <span data-ttu-id="cb770-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb770-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="cb770-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb770-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb770-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="cb770-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="cb770-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb770-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb770-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cb770-114">Not supported</span></span>                               |
| <span data-ttu-id="cb770-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="cb770-115">Application</span></span>                            | <span data-ttu-id="cb770-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb770-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb770-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb770-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/classes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb770-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cb770-118">Optional query parameters</span></span>

<span data-ttu-id="cb770-119">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в следующем примере:</span><span class="sxs-lookup"><span data-stu-id="cb770-119">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="cb770-120">Кроме того, для ограничения ответа можно использовать параметры и `$filter` `$count` `$search` параметры запросов.</span><span class="sxs-lookup"><span data-stu-id="cb770-120">You can also use the `$filter`, `$count` and `$search` query parameters to limit the response.</span></span> 

<span data-ttu-id="cb770-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="cb770-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="cb770-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="cb770-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="cb770-123">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cb770-123">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb770-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb770-124">Request headers</span></span>

| <span data-ttu-id="cb770-125">Имя</span><span class="sxs-lookup"><span data-stu-id="cb770-125">Name</span></span>          | <span data-ttu-id="cb770-126">Описание</span><span class="sxs-lookup"><span data-stu-id="cb770-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cb770-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb770-127">Authorization</span></span> | <span data-ttu-id="cb770-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb770-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb770-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb770-130">Request body</span></span>

<span data-ttu-id="cb770-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb770-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb770-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb770-132">Response</span></span>

<span data-ttu-id="cb770-133">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cb770-133">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb770-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="cb770-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb770-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb770-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_educationclass"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/classes
```

### <a name="response"></a><span data-ttu-id="cb770-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb770-136">Response</span></span>

> <span data-ttu-id="cb770-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cb770-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationClass)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationClass",
      "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
      "displayName": "String",
      "mailNickname": "String",
      "description": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "classCode": "String",
      "externalName": "String",
      "externalId": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "grade": "String",
      "term": {
        "@odata.type": "microsoft.graph.educationTerm"
      }
    }
  ]
}
```
