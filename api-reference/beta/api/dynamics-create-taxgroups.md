---
title: Создание Таксграупс
description: Создает объект налоговой группы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 6dfb5d68e18c92de4ecb702707b2fdc67fa5ea19
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458609"
---
# <a name="create-taxgroups"></a><span data-ttu-id="773a6-103">Создание Таксграупс</span><span class="sxs-lookup"><span data-stu-id="773a6-103">Create taxGroups</span></span>
<span data-ttu-id="773a6-104">Создайте объект налоговой группы в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="773a6-104">Create a tax groups object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="773a6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="773a6-105">Permissions</span></span>
<span data-ttu-id="773a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="773a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="773a6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="773a6-108">Permission type</span></span> |<span data-ttu-id="773a6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="773a6-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="773a6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="773a6-110">Delegated (work or school account)</span></span>|<span data-ttu-id="773a6-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="773a6-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="773a6-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="773a6-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="773a6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="773a6-113">Not supported.</span></span>|
|<span data-ttu-id="773a6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="773a6-114">Application</span></span>|<span data-ttu-id="773a6-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="773a6-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="773a6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="773a6-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/taxGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="773a6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="773a6-117">Optional query parameters</span></span>
<span data-ttu-id="773a6-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="773a6-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="773a6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="773a6-119">Request headers</span></span>

|<span data-ttu-id="773a6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="773a6-120">Header</span></span>|<span data-ttu-id="773a6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="773a6-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="773a6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="773a6-122">Authorization</span></span>  |<span data-ttu-id="773a6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="773a6-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="773a6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="773a6-125">Content-Type</span></span>  |<span data-ttu-id="773a6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="773a6-126">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="773a6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="773a6-127">Request body</span></span>
<span data-ttu-id="773a6-128">В тексте запроса добавьте представление объекта **Таксграупс** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="773a6-128">In the request body, supply a JSON representation of a **taxGroups** object.</span></span>

## <a name="response"></a><span data-ttu-id="773a6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="773a6-129">Response</span></span>
<span data-ttu-id="773a6-130">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **таксграупс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="773a6-130">If successful, this method returns ```201 Created``` response code and a **taxGroups** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="773a6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="773a6-131">Example</span></span>

<span data-ttu-id="773a6-132">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="773a6-132">**Request**</span></span>

<span data-ttu-id="773a6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="773a6-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/taxGroups
Content-type: application/json

{
  "code": "FURNITURE",
  "displayName": "Taxable Olympic Furniture",
  "taxType": "Sales Tax"
}
```

<span data-ttu-id="773a6-134">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="773a6-134">**Response**</span></span>

<span data-ttu-id="773a6-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="773a6-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="773a6-136">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="773a6-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="773a6-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="773a6-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "FURNITURE",
  "displayName": "Taxable Olympic Furniture",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-03-15T02:20:57.09Z"
}

```
