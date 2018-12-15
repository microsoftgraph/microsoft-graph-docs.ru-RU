---
title: 'пользователь: exportPersonalData'
description: Отправляет запрос операции данные политики, внесенные администратором компании для экспорта данных организации пользователя.
ms.openlocfilehash: 7d41d6d855fee992a4ff3a542e6c11f692adcfe3
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2018
ms.locfileid: "27284135"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="21ce7-103">пользователь: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="21ce7-103">user: exportPersonalData</span></span>

<span data-ttu-id="21ce7-104">Запрос данных политики операции от администратора компании или приложения для экспорта данных организации пользователя.</span><span class="sxs-lookup"><span data-stu-id="21ce7-104">Submit a data policy operation request from a company administrator or an application to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="21ce7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21ce7-105">Permissions</span></span>
<span data-ttu-id="21ce7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21ce7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21ce7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21ce7-108">Permission type</span></span>      | <span data-ttu-id="21ce7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21ce7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21ce7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21ce7-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="21ce7-111">User.Export.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="21ce7-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="21ce7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21ce7-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="21ce7-113">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="21ce7-113">Not applicable</span></span>  |
|<span data-ttu-id="21ce7-114">Application</span><span class="sxs-lookup"><span data-stu-id="21ce7-114">Application</span></span> | <span data-ttu-id="21ce7-115">User.Export.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="21ce7-115">User.Export.All, User.Read.All</span></span> |

><span data-ttu-id="21ce7-116">**Примечание:** Экспорт может выполняться только администратором компании при использовании делегированы разрешения.</span><span class="sxs-lookup"><span data-stu-id="21ce7-116">**Note:** The export can only be performed by a company administrator when delegated permissions are used.</span></span>

## <a name="http-request"></a><span data-ttu-id="21ce7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21ce7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="21ce7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21ce7-118">Request headers</span></span>
| <span data-ttu-id="21ce7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="21ce7-119">Name</span></span>       | <span data-ttu-id="21ce7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="21ce7-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="21ce7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="21ce7-121">Authorization</span></span>  | <span data-ttu-id="21ce7-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="21ce7-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="21ce7-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="21ce7-123">Request body</span></span>
<span data-ttu-id="21ce7-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="21ce7-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="21ce7-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="21ce7-125">Parameter</span></span>    | <span data-ttu-id="21ce7-126">Тип</span><span class="sxs-lookup"><span data-stu-id="21ce7-126">Type</span></span>   |<span data-ttu-id="21ce7-127">Описание</span><span class="sxs-lookup"><span data-stu-id="21ce7-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21ce7-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="21ce7-128">storageLocation</span></span>|<span data-ttu-id="21ce7-129">String.</span><span class="sxs-lookup"><span data-stu-id="21ce7-129">String</span></span>|<span data-ttu-id="21ce7-130">Это URL-адрес подписи (SAS) общий доступ к учетной записи хранилища Azure, для которых следует экспортировать данные.</span><span class="sxs-lookup"><span data-stu-id="21ce7-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="21ce7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="21ce7-131">Response</span></span>
<span data-ttu-id="21ce7-p102">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="21ce7-p102">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21ce7-134">Пример</span><span class="sxs-lookup"><span data-stu-id="21ce7-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21ce7-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="21ce7-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```

##### <a name="response"></a><span data-ttu-id="21ce7-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="21ce7-136">Response</span></span>
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
