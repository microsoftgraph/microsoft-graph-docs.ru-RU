---
title: 'пользователь: exportPersonalData'
description: Отправляет запрос операции данные политики, внесенные администратором компании для экспорта данных организации пользователя.
localization_priority: Normal
ms.openlocfilehash: d660994868e331fb8c1813bb9ff90aebe4790e9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845341"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="9ff1b-103">пользователь: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="9ff1b-103">user: exportPersonalData</span></span>

<span data-ttu-id="9ff1b-104">Отправляет запрос операции данные политики, сделанных с администратора компании для экспорта данных организации пользователя.</span><span class="sxs-lookup"><span data-stu-id="9ff1b-104">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ff1b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ff1b-105">Permissions</span></span>
<span data-ttu-id="9ff1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ff1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ff1b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ff1b-108">Permission type</span></span>      | <span data-ttu-id="9ff1b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ff1b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ff1b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ff1b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="9ff1b-111">User.Export.All и User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ff1b-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="9ff1b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ff1b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9ff1b-113">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="9ff1b-113">Not applicable</span></span>  |
|<span data-ttu-id="9ff1b-114">Application</span><span class="sxs-lookup"><span data-stu-id="9ff1b-114">Application</span></span> | <span data-ttu-id="9ff1b-115">User.Export.All и User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ff1b-115">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="9ff1b-116">**Примечание:** Экспорт может выполняться только администратором компании при использовании делегированных разрешений.</span><span class="sxs-lookup"><span data-stu-id="9ff1b-116">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="9ff1b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ff1b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="9ff1b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ff1b-118">Request headers</span></span>
| <span data-ttu-id="9ff1b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9ff1b-119">Name</span></span>       | <span data-ttu-id="9ff1b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9ff1b-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="9ff1b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ff1b-121">Authorization</span></span>  | <span data-ttu-id="9ff1b-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="9ff1b-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ff1b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9ff1b-123">Request body</span></span>
<span data-ttu-id="9ff1b-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9ff1b-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9ff1b-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="9ff1b-125">Parameter</span></span>    | <span data-ttu-id="9ff1b-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9ff1b-126">Type</span></span>   |<span data-ttu-id="9ff1b-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9ff1b-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9ff1b-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="9ff1b-128">storageLocation</span></span>|<span data-ttu-id="9ff1b-129">Строка</span><span class="sxs-lookup"><span data-stu-id="9ff1b-129">String</span></span>|<span data-ttu-id="9ff1b-130">Это URL-адрес подписи (SAS) общий доступ к учетной записи хранилища Azure, для которых следует экспортировать данные.</span><span class="sxs-lookup"><span data-stu-id="9ff1b-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="9ff1b-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ff1b-131">Response</span></span>
<span data-ttu-id="9ff1b-132">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="9ff1b-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="9ff1b-133">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9ff1b-133">It does not return anything in the response body.</span></span> <span data-ttu-id="9ff1b-134">Ответ содержит следующие заголовки.</span><span class="sxs-lookup"><span data-stu-id="9ff1b-134">The response contains the following headers.</span></span>

| <span data-ttu-id="9ff1b-135">Имя</span><span class="sxs-lookup"><span data-stu-id="9ff1b-135">Name</span></span>       | <span data-ttu-id="9ff1b-136">Описание</span><span class="sxs-lookup"><span data-stu-id="9ff1b-136">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="9ff1b-137">Расположение</span><span class="sxs-lookup"><span data-stu-id="9ff1b-137">Location</span></span>  | <span data-ttu-id="9ff1b-138">URL-адрес, чтобы проверить состояние запроса.</span><span class="sxs-lookup"><span data-stu-id="9ff1b-138">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="9ff1b-139">Повтор после</span><span class="sxs-lookup"><span data-stu-id="9ff1b-139">Retry-After</span></span>  | <span data-ttu-id="9ff1b-140">Период времени в секундах.</span><span class="sxs-lookup"><span data-stu-id="9ff1b-140">Time period in seconds.</span></span> <span data-ttu-id="9ff1b-141">Лиц, ответственных за запрос должен ожидать это время после отправки запроса для проверки состояния.</span><span class="sxs-lookup"><span data-stu-id="9ff1b-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="9ff1b-142">Пример</span><span class="sxs-lookup"><span data-stu-id="9ff1b-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ff1b-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ff1b-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
##### <a name="response"></a><span data-ttu-id="9ff1b-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ff1b-144">Response</span></span>

```
{
  Location: https://graph.microsoft.com/beta/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
