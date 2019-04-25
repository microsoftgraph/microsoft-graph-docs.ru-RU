---
title: 'Пользователь: Експортперсоналдата'
description: Передает запрос операции политики данных, сделанный администратором компании для экспорта данных пользователя организации.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7f112d065b75da7dc525e667df78b0264be37d55
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547902"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="4a006-103">Пользователь: Експортперсоналдата</span><span class="sxs-lookup"><span data-stu-id="4a006-103">user: exportPersonalData</span></span>

<span data-ttu-id="4a006-104">Передает запрос операции политики данных, сделанный администратором компании для экспорта данных пользователя организации.</span><span class="sxs-lookup"><span data-stu-id="4a006-104">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a006-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a006-105">Permissions</span></span>
<span data-ttu-id="4a006-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a006-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a006-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a006-108">Permission type</span></span>      | <span data-ttu-id="4a006-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a006-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a006-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a006-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4a006-111">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4a006-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="4a006-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a006-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4a006-113">Не применимо</span><span class="sxs-lookup"><span data-stu-id="4a006-113">Not applicable</span></span>  |
|<span data-ttu-id="4a006-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a006-114">Application</span></span> | <span data-ttu-id="4a006-115">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4a006-115">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="4a006-116">**Примечание:** Экспорт может выполняться только администратором компании при использовании делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="4a006-116">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="4a006-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a006-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="4a006-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a006-118">Request headers</span></span>
| <span data-ttu-id="4a006-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4a006-119">Name</span></span>       | <span data-ttu-id="4a006-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4a006-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4a006-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a006-121">Authorization</span></span>  | <span data-ttu-id="4a006-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="4a006-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a006-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a006-123">Request body</span></span>
<span data-ttu-id="4a006-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4a006-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4a006-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="4a006-125">Parameter</span></span>    | <span data-ttu-id="4a006-126">Тип</span><span class="sxs-lookup"><span data-stu-id="4a006-126">Type</span></span>   |<span data-ttu-id="4a006-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4a006-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4a006-128">Сторажелокатион</span><span class="sxs-lookup"><span data-stu-id="4a006-128">storageLocation</span></span>|<span data-ttu-id="4a006-129">String</span><span class="sxs-lookup"><span data-stu-id="4a006-129">String</span></span>|<span data-ttu-id="4a006-130">Это URL-адрес учетной записи службы хранилища Azure, в которую будут экспортироваться данные.</span><span class="sxs-lookup"><span data-stu-id="4a006-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="4a006-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a006-131">Response</span></span>
<span data-ttu-id="4a006-132">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="4a006-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="4a006-133">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4a006-133">It does not return anything in the response body.</span></span> <span data-ttu-id="4a006-134">Ответ содержит следующие заголовки.</span><span class="sxs-lookup"><span data-stu-id="4a006-134">The response contains the following headers.</span></span>

| <span data-ttu-id="4a006-135">Имя</span><span class="sxs-lookup"><span data-stu-id="4a006-135">Name</span></span>       | <span data-ttu-id="4a006-136">Описание</span><span class="sxs-lookup"><span data-stu-id="4a006-136">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4a006-137">Location</span><span class="sxs-lookup"><span data-stu-id="4a006-137">Location</span></span>  | <span data-ttu-id="4a006-138">URL-адрес для проверки состояния запроса.</span><span class="sxs-lookup"><span data-stu-id="4a006-138">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="4a006-139">Retry — после</span><span class="sxs-lookup"><span data-stu-id="4a006-139">Retry-After</span></span>  | <span data-ttu-id="4a006-140">Период времени в секундах.</span><span class="sxs-lookup"><span data-stu-id="4a006-140">Time period in seconds.</span></span> <span data-ttu-id="4a006-141">Запрос должен подождать этого времени после отправки запроса на проверку состояния.</span><span class="sxs-lookup"><span data-stu-id="4a006-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="4a006-142">Пример</span><span class="sxs-lookup"><span data-stu-id="4a006-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a006-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a006-143">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="4a006-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a006-144">Response</span></span>

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
