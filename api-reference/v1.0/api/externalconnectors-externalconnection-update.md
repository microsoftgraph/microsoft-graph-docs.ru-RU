---
title: Обновление externalConnection
description: Обновление свойств объекта externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 4dc8c4ff93b160b34028aee250eb1b7f6f0cc86d
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467462"
---
# <a name="update-externalconnection"></a><span data-ttu-id="d95d7-103">Обновление externalConnection</span><span class="sxs-lookup"><span data-stu-id="d95d7-103">Update externalConnection</span></span>

<span data-ttu-id="d95d7-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="d95d7-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="d95d7-105">Обновление свойств объекта [externalConnection.](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="d95d7-105">Update the properties of an [externalConnection](../resources/externalconnectors-externalconnection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d95d7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d95d7-106">Permissions</span></span>
<span data-ttu-id="d95d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d95d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d95d7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d95d7-109">Permission type</span></span>                        | <span data-ttu-id="d95d7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d95d7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d95d7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d95d7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d95d7-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d95d7-112">Not supported.</span></span> |
| <span data-ttu-id="d95d7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d95d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d95d7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d95d7-114">Not supported.</span></span> |
| <span data-ttu-id="d95d7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d95d7-115">Application</span></span>                            | <span data-ttu-id="d95d7-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="d95d7-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="d95d7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d95d7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /connections/{connectionsId}
```

## <a name="request-headers"></a><span data-ttu-id="d95d7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d95d7-118">Request headers</span></span>

| <span data-ttu-id="d95d7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d95d7-119">Name</span></span>          | <span data-ttu-id="d95d7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d95d7-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="d95d7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d95d7-121">Authorization</span></span> | <span data-ttu-id="d95d7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d95d7-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d95d7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d95d7-124">Content-Type</span></span>  | <span data-ttu-id="d95d7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d95d7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d95d7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d95d7-127">Request body</span></span>
<span data-ttu-id="d95d7-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d95d7-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d95d7-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="d95d7-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d95d7-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d95d7-130">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="d95d7-131">Могут быть обновлены перечисленные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="d95d7-131">The following properties can be updated.</span></span>

| <span data-ttu-id="d95d7-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="d95d7-132">Property</span></span>      | <span data-ttu-id="d95d7-133">Тип</span><span class="sxs-lookup"><span data-stu-id="d95d7-133">Type</span></span>                                           | <span data-ttu-id="d95d7-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d95d7-134">Description</span></span> |
|:--------------|:-----------------------------------------------|:------------|
| <span data-ttu-id="d95d7-135">configuration</span><span class="sxs-lookup"><span data-stu-id="d95d7-135">configuration</span></span> | [<span data-ttu-id="d95d7-136">microsoft.graph.externalConnectors.configuration</span><span class="sxs-lookup"><span data-stu-id="d95d7-136">microsoft.graph.externalConnectors.configuration</span></span>](../resources/externalconnectors-configuration.md) | <span data-ttu-id="d95d7-137">Указывает дополнительные ID-адреса приложений, которые разрешены для управления подключением и индексации контента в подключении.</span><span class="sxs-lookup"><span data-stu-id="d95d7-137">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> |
| <span data-ttu-id="d95d7-138">description</span><span class="sxs-lookup"><span data-stu-id="d95d7-138">description</span></span>   | <span data-ttu-id="d95d7-139">String</span><span class="sxs-lookup"><span data-stu-id="d95d7-139">String</span></span>                                         | <span data-ttu-id="d95d7-140">Описание подключения, отображаемого в Центр администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d95d7-140">Description of the connection displayed in the Microsoft 365 admin center.</span></span> |
| <span data-ttu-id="d95d7-141">name</span><span class="sxs-lookup"><span data-stu-id="d95d7-141">name</span></span>          | <span data-ttu-id="d95d7-142">String</span><span class="sxs-lookup"><span data-stu-id="d95d7-142">String</span></span>                                         | <span data-ttu-id="d95d7-143">Отображает имя подключения, отображаемого в Центр администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d95d7-143">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="d95d7-144">Максимальная длина 128 символов.</span><span class="sxs-lookup"><span data-stu-id="d95d7-144">Maximum length of 128 characters.</span></span> |


## <a name="response"></a><span data-ttu-id="d95d7-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d95d7-145">Response</span></span>

<span data-ttu-id="d95d7-146">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d95d7-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d95d7-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="d95d7-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d95d7-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="d95d7-148">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_externalconnection"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/connections/contosohr
Content-type: application/json

{
  "name": "Contoso HR Service Tickets",
  "description": "Connection to index HR service tickets"
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="d95d7-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d95d7-149">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="d95d7-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d95d7-150">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```