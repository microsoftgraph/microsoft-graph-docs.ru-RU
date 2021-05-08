---
title: 'educationSchool: delta'
description: Создайте новые или обновленные школы, не выполняя полное чтение всей школьной коллекции.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3604a9296d7419d20e1b2b9016a2dc724b65c222
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232278"
---
# <a name="educationschool-delta"></a><span data-ttu-id="21e1e-103">educationSchool: delta</span><span class="sxs-lookup"><span data-stu-id="21e1e-103">educationSchool: delta</span></span>

<span data-ttu-id="21e1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21e1e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="21e1e-105">Создайте новые или обновленные школы, не выполняя полное чтение всей школьной коллекции.</span><span class="sxs-lookup"><span data-stu-id="21e1e-105">Get newly created or updated schools without having to perform a full read of the entire school collection.</span></span> <span data-ttu-id="21e1e-106">Подробные [сведения см. в запросе Use Delta.](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="21e1e-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="21e1e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21e1e-107">Permissions</span></span>

<span data-ttu-id="21e1e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21e1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="21e1e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21e1e-110">Permission type</span></span>                        | <span data-ttu-id="21e1e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21e1e-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="21e1e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21e1e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="21e1e-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="21e1e-113">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="21e1e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21e1e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21e1e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21e1e-115">Not supported.</span></span>                              |
| <span data-ttu-id="21e1e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="21e1e-116">Application</span></span>                            | <span data-ttu-id="21e1e-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21e1e-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="21e1e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21e1e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/delta
```

## <a name="request-headers"></a><span data-ttu-id="21e1e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21e1e-119">Request headers</span></span>

| <span data-ttu-id="21e1e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="21e1e-120">Name</span></span>          | <span data-ttu-id="21e1e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="21e1e-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="21e1e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21e1e-122">Authorization</span></span> | <span data-ttu-id="21e1e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21e1e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21e1e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21e1e-125">Request body</span></span>

<span data-ttu-id="21e1e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21e1e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21e1e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="21e1e-127">Response</span></span>

<span data-ttu-id="21e1e-128">В случае успешной работы эта функция возвращает код отклика и `200 OK` [коллекцию educationSchool](../resources/educationschool.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="21e1e-128">If successful, this function returns a `200 OK` response code and a [educationSchool](../resources/educationschool.md) collection in the response body.</span></span> <span data-ttu-id="21e1e-129">Отклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="21e1e-129">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="21e1e-130">Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="21e1e-130">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="21e1e-131">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="21e1e-131">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="21e1e-132">Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="21e1e-132">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="21e1e-133">Сохраните и используйте `deltaLink` URL-адрес, чтобы узнать об изменениях в ресурсе в будущем.</span><span class="sxs-lookup"><span data-stu-id="21e1e-133">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="21e1e-134">Подробные сведения см. в [материале Использование запроса delta.](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="21e1e-134">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="21e1e-135">Например, запросы см. [в рублях Получить дополнительные изменения для пользователей.](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="21e1e-135">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="examples"></a><span data-ttu-id="21e1e-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="21e1e-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="21e1e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="21e1e-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/schools/delta
```

### <a name="response"></a><span data-ttu-id="21e1e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="21e1e-138">Response</span></span>

> <span data-ttu-id="21e1e-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="21e1e-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationSchool)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationSchool)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/education/schools/delta?$skiptoken=VwhMSQw1l1O5v2F1ZPm...",
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationSchool",
      "id": "String (identifier)",
      "displayName": "String",
      "description": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "principalEmail": "String",
      "principalName": "String",
      "externalPrincipalId": "String",
      "lowestGrade": "String",
      "highestGrade": "String",
      "schoolNumber": "String",
      "externalId": "String",
      "phone": "String",
      "fax": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "address": {
        "@odata.type": "microsoft.graph.physicalAddress"
      }
    }
  ]
}
```
