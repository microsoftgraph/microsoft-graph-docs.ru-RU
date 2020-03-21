---
title: Обновление параметров
description: Обновление параметров на уровне клиента для универсальной службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a51a9e2a50b2a5625f099103aeb23bb97b93fcf8
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896334"
---
# <a name="update-settings"></a><span data-ttu-id="293ab-103">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="293ab-103">Update settings</span></span>

<span data-ttu-id="293ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="293ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="293ab-105">Обновление параметров на уровне клиента для универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="293ab-105">Update tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="293ab-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="293ab-106">Permissions</span></span>
<span data-ttu-id="293ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="293ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="293ab-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="293ab-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="293ab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="293ab-110">Permission type</span></span> | <span data-ttu-id="293ab-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="293ab-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="293ab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="293ab-112">Delegated (work or school account)</span></span>| <span data-ttu-id="293ab-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="293ab-113">Users.Read.All</span></span> |
|<span data-ttu-id="293ab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="293ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="293ab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="293ab-115">Not Supported.</span></span>|
|<span data-ttu-id="293ab-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="293ab-116">Application</span></span>|<span data-ttu-id="293ab-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="293ab-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="293ab-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="293ab-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/settings
```

## <a name="optional-request-headers"></a><span data-ttu-id="293ab-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="293ab-119">Optional request headers</span></span>
| <span data-ttu-id="293ab-120">Имя</span><span class="sxs-lookup"><span data-stu-id="293ab-120">Name</span></span>       | <span data-ttu-id="293ab-121">Описание</span><span class="sxs-lookup"><span data-stu-id="293ab-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="293ab-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="293ab-122">Authorization</span></span> | <span data-ttu-id="293ab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="293ab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="293ab-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="293ab-125">Content-type</span></span>  | <span data-ttu-id="293ab-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="293ab-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="293ab-128">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="293ab-128">Request body</span></span>
<span data-ttu-id="293ab-129">В тексте запроса укажите значения для соответствующих полей [принтсеттингс](../resources/printsettings.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="293ab-129">In the request body, supply the values for the relevant [printSettings](../resources/printsettings.md) fields that should be updated.</span></span> <span data-ttu-id="293ab-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="293ab-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="293ab-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="293ab-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="293ab-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="293ab-132">Property</span></span>     | <span data-ttu-id="293ab-133">Тип</span><span class="sxs-lookup"><span data-stu-id="293ab-133">Type</span></span>        | <span data-ttu-id="293ab-134">Описание</span><span class="sxs-lookup"><span data-stu-id="293ab-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="293ab-135">документконверсионенаблед</span><span class="sxs-lookup"><span data-stu-id="293ab-135">documentConversionEnabled</span></span>|<span data-ttu-id="293ab-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="293ab-136">Boolean</span></span>|<span data-ttu-id="293ab-137">Указывает, включено ли преобразование документов для клиента.</span><span class="sxs-lookup"><span data-stu-id="293ab-137">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="293ab-138">Если включено преобразование документов, то при необходимости в универсальной службе печати документы автоматически преобразуются в формат, совместимый с принтером (например, XPS — PDF).</span><span class="sxs-lookup"><span data-stu-id="293ab-138">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (for example, XPS to PDF) when needed.</span></span>|

## <a name="response"></a><span data-ttu-id="293ab-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="293ab-139">Response</span></span>
<span data-ttu-id="293ab-140">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="293ab-140">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="293ab-141">Пример</span><span class="sxs-lookup"><span data-stu-id="293ab-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="293ab-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="293ab-142">Request</span></span>
<span data-ttu-id="293ab-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="293ab-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_settings"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/settings
Content-type: application/json

{
  "documentConversionEnabled": true
}
```
##### <a name="response"></a><span data-ttu-id="293ab-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="293ab-144">Response</span></span>
<span data-ttu-id="293ab-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="293ab-145">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings"
} -->
```http
HTTP/1.1 204 NoContent
Content-length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->