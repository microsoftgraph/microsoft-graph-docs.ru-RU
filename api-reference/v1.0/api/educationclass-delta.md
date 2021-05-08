---
title: 'educationClass: delta'
description: Получите новые или обновленные классы, в том числе изменения членства, без выполнения полного чтения всей коллекции классов.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 80ca48a1494281fed4a39dfff342233a268b5122
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232270"
---
# <a name="educationclass-delta"></a><span data-ttu-id="266d3-103">educationClass: delta</span><span class="sxs-lookup"><span data-stu-id="266d3-103">educationClass: delta</span></span>

<span data-ttu-id="266d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="266d3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="266d3-105">Получите новые или обновленные классы, в том числе изменения членства, без выполнения полного чтения всей коллекции классов.</span><span class="sxs-lookup"><span data-stu-id="266d3-105">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span></span> <span data-ttu-id="266d3-106">Подробные [сведения см. в запросе Use Delta.](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="266d3-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="266d3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="266d3-107">Permissions</span></span>

<span data-ttu-id="266d3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="266d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="266d3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="266d3-110">Permission type</span></span>                        | <span data-ttu-id="266d3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="266d3-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="266d3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="266d3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="266d3-113">EduRoster.ReadBasic, EduRoster.Read или EduRoster.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="266d3-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="266d3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="266d3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="266d3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="266d3-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="266d3-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="266d3-116">Application</span></span>                            | <span data-ttu-id="266d3-117">EduRoster.ReadBasic.All, EduRoster.Read.All или EduRoster.WriteWrite.All</span><span class="sxs-lookup"><span data-stu-id="266d3-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="266d3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="266d3-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/classes/delta
```

## <a name="request-headers"></a><span data-ttu-id="266d3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="266d3-119">Request headers</span></span>

| <span data-ttu-id="266d3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="266d3-120">Name</span></span>          | <span data-ttu-id="266d3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="266d3-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="266d3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="266d3-122">Authorization</span></span> | <span data-ttu-id="266d3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="266d3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="266d3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="266d3-125">Request body</span></span>

<span data-ttu-id="266d3-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="266d3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="266d3-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="266d3-127">Response</span></span>

<span data-ttu-id="266d3-128">В случае успешной работы эта функция возвращает код ответа и `200 OK` коллекцию [educationClass](../resources/educationclass.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="266d3-128">If successful, this function returns an `200 OK` response code and an [educationClass](../resources/educationclass.md) collection in the response body.</span></span> <span data-ttu-id="266d3-129">Отклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="266d3-129">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="266d3-130">Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="266d3-130">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="266d3-131">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="266d3-131">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="266d3-132">Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="266d3-132">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="266d3-133">Сохраните и используйте `deltaLink` URL-адрес, чтобы узнать об изменениях в ресурсе в будущем.</span><span class="sxs-lookup"><span data-stu-id="266d3-133">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="266d3-134">Подробные сведения см. в [материале Использование запроса delta.](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="266d3-134">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="266d3-135">Например, запросы см. [в рублях Получить дополнительные изменения для пользователей.](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="266d3-135">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="266d3-136">дельты educationClass не включают удаленные классы.</span><span class="sxs-lookup"><span data-stu-id="266d3-136">educationClass deltas do not include deleted classes.</span></span>

## <a name="examples"></a><span data-ttu-id="266d3-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="266d3-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="266d3-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="266d3-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/classes/delta
```

### <a name="response"></a><span data-ttu-id="266d3-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="266d3-139">Response</span></span>

> <span data-ttu-id="266d3-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="266d3-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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

  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationClass)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/education/classes/delta?$skiptoken=sU1S4IJGk3hwxbia8...",
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationClass",
      "id": "String (identifier)",
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
