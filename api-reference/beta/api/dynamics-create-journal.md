---
title: Создание журналов
description: Создает объект журнала в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 27bef92d9392cd6369564e86417b438ed8bd5a5a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463637"
---
# <a name="create-journals"></a><span data-ttu-id="d1c54-103">Создание журналов</span><span class="sxs-lookup"><span data-stu-id="d1c54-103">Create journals</span></span>
<span data-ttu-id="d1c54-104">Создает журнал в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="d1c54-104">Creates a journal in Dynamics 365 Business Central.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d1c54-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1c54-105">Permissions</span></span>
<span data-ttu-id="d1c54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1c54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1c54-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1c54-108">Permission type</span></span> |<span data-ttu-id="d1c54-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1c54-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d1c54-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1c54-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d1c54-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1c54-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d1c54-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1c54-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d1c54-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1c54-113">Not supported.</span></span>|
|<span data-ttu-id="d1c54-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1c54-114">Application</span></span>|<span data-ttu-id="d1c54-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1c54-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1c54-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1c54-116">HTTP request</span></span>

```
POST /financials/companies('{id}')/journals('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1c54-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d1c54-117">Optional query parameters</span></span>
<span data-ttu-id="d1c54-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d1c54-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1c54-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1c54-119">Request headers</span></span>
|<span data-ttu-id="d1c54-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1c54-120">Header</span></span>        |<span data-ttu-id="d1c54-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d1c54-121">Value</span></span>                     |
|--------------|--------------------------|
|<span data-ttu-id="d1c54-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1c54-122">Authorization</span></span> |<span data-ttu-id="d1c54-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1c54-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="d1c54-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1c54-125">Content-Type</span></span>  |<span data-ttu-id="d1c54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1c54-126">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="d1c54-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1c54-127">Request body</span></span>
<span data-ttu-id="d1c54-128">В тексте запроса добавьте представление объекта **журналов** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1c54-128">In the request body, supply a JSON representation of a **journals** object.</span></span>

## <a name="response"></a><span data-ttu-id="d1c54-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1c54-129">Response</span></span>
<span data-ttu-id="d1c54-130">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **журналов** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1c54-130">If successful, this method returns ```201 Created``` response code and a **journals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1c54-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d1c54-131">Example</span></span>

<span data-ttu-id="d1c54-132">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="d1c54-132">**Request**</span></span>

<span data-ttu-id="d1c54-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1c54-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/journals
Content-type: application/json

```json
{
  "code": "DEFAULT"
}
```

<span data-ttu-id="d1c54-134">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="d1c54-134">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```

