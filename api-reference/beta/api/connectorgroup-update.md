---
title: Обновление Коннекторграупс
description: Обновление свойств объекта коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 80565045fa292b09e5c8e98544c466ec784f24f0
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44555808"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="5d020-103">Обновление Коннекторграупс</span><span class="sxs-lookup"><span data-stu-id="5d020-103">Update connectorGroups</span></span>

<span data-ttu-id="5d020-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d020-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d020-105">Обновление свойств объекта [коннекторграуп](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="5d020-105">Update the properties of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d020-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d020-106">Permissions</span></span>
<span data-ttu-id="5d020-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d020-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d020-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d020-109">Permission type</span></span>      | <span data-ttu-id="5d020-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d020-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d020-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d020-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5d020-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5d020-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5d020-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d020-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d020-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d020-114">Not supported.</span></span>    |
|<span data-ttu-id="5d020-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="5d020-115">Application</span></span> | <span data-ttu-id="5d020-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d020-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d020-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d020-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="5d020-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d020-118">Optional request headers</span></span>
| <span data-ttu-id="5d020-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5d020-119">Name</span></span>       | <span data-ttu-id="5d020-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5d020-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5d020-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d020-121">Authorization</span></span>  | <span data-ttu-id="5d020-122">Носителя.</span><span class="sxs-lookup"><span data-stu-id="5d020-122">Bearer.</span></span> <span data-ttu-id="5d020-123">Обязательное</span><span class="sxs-lookup"><span data-stu-id="5d020-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d020-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d020-124">Request body</span></span>
<span data-ttu-id="5d020-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5d020-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5d020-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d020-128">Property</span></span>     | <span data-ttu-id="5d020-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5d020-129">Type</span></span>   |<span data-ttu-id="5d020-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5d020-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d020-131">коннекторграуптипе</span><span class="sxs-lookup"><span data-stu-id="5d020-131">connectorGroupType</span></span>|<span data-ttu-id="5d020-132">string</span><span class="sxs-lookup"><span data-stu-id="5d020-132">string</span></span>| <span data-ttu-id="5d020-133">Указывает тип гибридного агента.</span><span class="sxs-lookup"><span data-stu-id="5d020-133">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="5d020-134">Это предварительно заданное системой.</span><span class="sxs-lookup"><span data-stu-id="5d020-134">This pre-set by the system.</span></span> |
|<span data-ttu-id="5d020-135">id</span><span class="sxs-lookup"><span data-stu-id="5d020-135">id</span></span>|<span data-ttu-id="5d020-136">строка</span><span class="sxs-lookup"><span data-stu-id="5d020-136">string</span></span>| <span data-ttu-id="5d020-137">Уникальный идентификатор для этого Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="5d020-137">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="5d020-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d020-138">Read-only.</span></span> |
|<span data-ttu-id="5d020-139">isDefault</span><span class="sxs-lookup"><span data-stu-id="5d020-139">isDefault</span></span>|<span data-ttu-id="5d020-140">boolean</span><span class="sxs-lookup"><span data-stu-id="5d020-140">boolean</span></span>| <span data-ttu-id="5d020-141">Указывает, является ли Коннекторграуп Коннекторграуп по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5d020-141">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="5d020-142">Только одна группа соединителей может быть Коннекторграуп по умолчанию, и она предопределена системой.</span><span class="sxs-lookup"><span data-stu-id="5d020-142">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> |
|<span data-ttu-id="5d020-143">name</span><span class="sxs-lookup"><span data-stu-id="5d020-143">name</span></span>|<span data-ttu-id="5d020-144">string</span><span class="sxs-lookup"><span data-stu-id="5d020-144">string</span></span>| <span data-ttu-id="5d020-145">Имя, связанное с Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="5d020-145">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="5d020-146">региональных</span><span class="sxs-lookup"><span data-stu-id="5d020-146">region</span></span>|<span data-ttu-id="5d020-147">string</span><span class="sxs-lookup"><span data-stu-id="5d020-147">string</span></span>| <span data-ttu-id="5d020-148">Регион, которому назначена Коннекторграуп, и который оптимизирует трафик для.</span><span class="sxs-lookup"><span data-stu-id="5d020-148">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="5d020-149">Эту область можно задать только в том случае, если Коннекторграуп **не назначен ни один** из соединителей или приложений.</span><span class="sxs-lookup"><span data-stu-id="5d020-149">This region can only be set if **no** connectors or applications are assigned to the connectorGroup.</span></span> <span data-ttu-id="5d020-150">Доступны следующие регионы: Северная Америка, Европа, Австралия, Азия и Индии.</span><span class="sxs-lookup"><span data-stu-id="5d020-150">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="5d020-151">Возможные значения: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="5d020-151">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="response"></a><span data-ttu-id="5d020-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d020-152">Response</span></span>

<span data-ttu-id="5d020-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [коннекторграуп](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5d020-153">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d020-154">Пример</span><span class="sxs-lookup"><span data-stu-id="5d020-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d020-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d020-155">Request</span></span>
<span data-ttu-id="5d020-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d020-156">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "region": "region-value"
}
```
##### <a name="response"></a><span data-ttu-id="5d020-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d020-157">Response</span></span>
<span data-ttu-id="5d020-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5d020-158">The following is an example of the response.</span></span> <span data-ttu-id="5d020-159">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="5d020-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5d020-160">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d020-160">All of the properties will be returned from an actual call.</span></span>
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
  "isDefault": true,
  "region": "region-value"
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
