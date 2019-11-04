---
title: Обновление Екстерналконнектион
description: Обновление свойств объекта Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 3caef56676060c37c092aed63bf12a4939bd551e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938648"
---
# <a name="update-connection"></a><span data-ttu-id="d012e-103">Обновление подключения</span><span class="sxs-lookup"><span data-stu-id="d012e-103">Update connection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d012e-104">Обновление свойств объекта [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="d012e-104">Update the properties of an [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d012e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d012e-105">Permissions</span></span>

<span data-ttu-id="d012e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d012e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d012e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d012e-108">Permission type</span></span>                        | <span data-ttu-id="d012e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d012e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d012e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d012e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d012e-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d012e-111">Not supported.</span></span> |
| <span data-ttu-id="d012e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d012e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d012e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d012e-113">Not supported.</span></span> |
| <span data-ttu-id="d012e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d012e-114">Application</span></span>                            | <span data-ttu-id="d012e-115">Екстерналитем. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d012e-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d012e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d012e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d012e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d012e-117">Request headers</span></span>

| <span data-ttu-id="d012e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d012e-118">Name</span></span>          | <span data-ttu-id="d012e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d012e-119">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="d012e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d012e-120">Authorization</span></span> | <span data-ttu-id="d012e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d012e-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d012e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d012e-123">Content-Type</span></span>  | <span data-ttu-id="d012e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d012e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d012e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d012e-126">Request body</span></span>

<span data-ttu-id="d012e-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d012e-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d012e-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="d012e-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d012e-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d012e-129">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="d012e-130">Могут быть обновлены перечисленные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="d012e-130">The following properties can be updated.</span></span>

| <span data-ttu-id="d012e-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="d012e-131">Property</span></span>      | <span data-ttu-id="d012e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d012e-132">Type</span></span>                                           | <span data-ttu-id="d012e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d012e-133">Description</span></span> |
|:--------------|:-----------------------------------------------|:------------|
| <span data-ttu-id="d012e-134">конфигурацион</span><span class="sxs-lookup"><span data-stu-id="d012e-134">configuration</span></span> | [<span data-ttu-id="d012e-135">configuration</span><span class="sxs-lookup"><span data-stu-id="d012e-135">configuration</span></span>](../resources/configuration.md) | <span data-ttu-id="d012e-136">Задает дополнительные идентификаторы приложений, которым разрешено управлять подключением и индексировать содержимое в подключении.</span><span class="sxs-lookup"><span data-stu-id="d012e-136">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> |
| <span data-ttu-id="d012e-137">description</span><span class="sxs-lookup"><span data-stu-id="d012e-137">description</span></span>   | <span data-ttu-id="d012e-138">String</span><span class="sxs-lookup"><span data-stu-id="d012e-138">String</span></span>                                         | <span data-ttu-id="d012e-139">Описание подключения, отображаемое в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d012e-139">Description of the connection displayed in the Microsoft 365 admin center.</span></span> |
| <span data-ttu-id="d012e-140">name</span><span class="sxs-lookup"><span data-stu-id="d012e-140">name</span></span>          | <span data-ttu-id="d012e-141">String</span><span class="sxs-lookup"><span data-stu-id="d012e-141">String</span></span>                                         | <span data-ttu-id="d012e-142">Отображаемое имя подключения, отображаемое в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d012e-142">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="d012e-143">Максимальная длина 128 символов.</span><span class="sxs-lookup"><span data-stu-id="d012e-143">Maximum length of 128 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="d012e-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="d012e-144">Response</span></span>

<span data-ttu-id="d012e-145">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d012e-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d012e-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="d012e-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d012e-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="d012e-147">Request</span></span>

<span data-ttu-id="d012e-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d012e-148">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connection"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr
Content-type: application/json

{
  "name": "Contoso HR Service Tickets",
  "description": "Connection to index HR service tickets"
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="d012e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d012e-149">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="d012e-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d012e-150">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update connection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
