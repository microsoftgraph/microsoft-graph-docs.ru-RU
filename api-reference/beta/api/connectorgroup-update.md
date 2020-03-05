---
title: Обновление Коннекторграупс
description: Обновление свойств объекта коннекторграуп.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: ad83631d6707e5f72f0813a71f7e40497e1903b0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437177"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="3e585-103">Обновление Коннекторграупс</span><span class="sxs-lookup"><span data-stu-id="3e585-103">Update connectorGroups</span></span>

<span data-ttu-id="3e585-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3e585-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e585-105">Обновление свойств объекта коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="3e585-105">Update the properties of connectorgroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e585-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e585-106">Permissions</span></span>
<span data-ttu-id="3e585-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e585-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e585-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e585-109">Permission type</span></span>      | <span data-ttu-id="3e585-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e585-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e585-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e585-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3e585-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3e585-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3e585-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e585-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e585-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e585-114">Not supported.</span></span>    |
|<span data-ttu-id="3e585-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e585-115">Application</span></span> | <span data-ttu-id="3e585-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e585-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e585-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e585-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3e585-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e585-118">Optional request headers</span></span>
| <span data-ttu-id="3e585-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3e585-119">Name</span></span>       | <span data-ttu-id="3e585-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3e585-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3e585-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e585-121">Authorization</span></span>  | <span data-ttu-id="3e585-122">Носителя.</span><span class="sxs-lookup"><span data-stu-id="3e585-122">Bearer.</span></span> <span data-ttu-id="3e585-123">Обязательна</span><span class="sxs-lookup"><span data-stu-id="3e585-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e585-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e585-124">Request body</span></span>
<span data-ttu-id="3e585-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3e585-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3e585-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e585-128">Property</span></span>     | <span data-ttu-id="3e585-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3e585-129">Type</span></span>   |<span data-ttu-id="3e585-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3e585-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e585-131">коннекторграуптипе</span><span class="sxs-lookup"><span data-stu-id="3e585-131">connectorGroupType</span></span>|<span data-ttu-id="3e585-132">строка</span><span class="sxs-lookup"><span data-stu-id="3e585-132">string</span></span>| <span data-ttu-id="3e585-133">Возможные значения: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="3e585-133">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="3e585-134">name</span><span class="sxs-lookup"><span data-stu-id="3e585-134">name</span></span>|<span data-ttu-id="3e585-135">String</span><span class="sxs-lookup"><span data-stu-id="3e585-135">String</span></span>|<span data-ttu-id="3e585-136">Имя Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="3e585-136">The name of the connectorGroup.</span></span>|

## <a name="response"></a><span data-ttu-id="3e585-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e585-137">Response</span></span>

<span data-ttu-id="3e585-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [коннекторграуп](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e585-138">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e585-139">Пример</span><span class="sxs-lookup"><span data-stu-id="3e585-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e585-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e585-140">Request</span></span>
<span data-ttu-id="3e585-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e585-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
PATCH https://graph.microsoft.com/{ver}/connectorGroups/{id}
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
}
```
##### <a name="response"></a><span data-ttu-id="3e585-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e585-142">Response</span></span>
<span data-ttu-id="3e585-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e585-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
