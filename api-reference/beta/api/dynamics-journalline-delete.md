---
title: Удаление Жаурналлинес
description: Удаляет строку журнала в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: c65a742d617818b2d25b936cbd9ba8eb0fc63d83
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458308"
---
# <a name="delete-journallines"></a><span data-ttu-id="5703c-103">Удаление Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="5703c-103">Delete journalLines</span></span>
<span data-ttu-id="5703c-104">Удаление объекта строки журнала из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="5703c-104">Delete a journal line object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="5703c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5703c-105">Permissions</span></span>
<span data-ttu-id="5703c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5703c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5703c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5703c-108">Permission type</span></span> |<span data-ttu-id="5703c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5703c-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="5703c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5703c-110">Delegated (work or school account)</span></span>|<span data-ttu-id="5703c-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5703c-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="5703c-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5703c-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5703c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5703c-113">Not supported.</span></span>|
|<span data-ttu-id="5703c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5703c-114">Application</span></span>|<span data-ttu-id="5703c-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5703c-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5703c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5703c-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/journals('{id}')/journalLines('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5703c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5703c-117">Optional query parameters</span></span>
<span data-ttu-id="5703c-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5703c-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5703c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5703c-119">Request headers</span></span>
|<span data-ttu-id="5703c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5703c-120">Header</span></span>          |<span data-ttu-id="5703c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5703c-121">Value</span></span>                     |
|----------------|--------------------------|
|<span data-ttu-id="5703c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5703c-122">Authorization</span></span>   |<span data-ttu-id="5703c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5703c-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="5703c-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="5703c-125">If-Match</span></span>        |<span data-ttu-id="5703c-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="5703c-126">Required.</span></span> <span data-ttu-id="5703c-127">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **жаурналлинес**, **жаурналлинес** не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="5703c-127">When this request header is included and the eTag provided does not match the current tag on the **journalLines**, the **journalLines** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5703c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5703c-128">Request body</span></span>

<span data-ttu-id="5703c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5703c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5703c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5703c-130">Response</span></span>

<span data-ttu-id="5703c-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5703c-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5703c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5703c-133">Example</span></span>

<span data-ttu-id="5703c-134">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="5703c-134">**Request**</span></span>

<span data-ttu-id="5703c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5703c-135">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/journals('{id}')/journalLines('{id}')
```

<span data-ttu-id="5703c-136">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="5703c-136">**Response**</span></span> 

<span data-ttu-id="5703c-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5703c-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
