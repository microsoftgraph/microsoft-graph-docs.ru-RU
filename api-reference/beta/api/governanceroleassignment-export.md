---
title: Экспорт Говернанцеролеассигнментрекуестс
description: Получение коллекции Говернанцеролеассигнментрекуестс в формате `application/octet-stream` , который можно проанализировать как CSV-файл в браузере.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: d37ef5fb09e937835dfe496717b58b3934ee606b
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635058"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="d959c-103">Экспорт Говернанцеролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="d959c-103">Export governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="d959c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d959c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d959c-105">Получение коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) в формате `application/octet-stream` , который можно проанализировать как CSV-файл в браузере.</span><span class="sxs-lookup"><span data-stu-id="d959c-105">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="d959c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d959c-106">Permissions</span></span>
<span data-ttu-id="d959c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="d959c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="d959c-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="d959c-109">Azure resources</span></span>

| <span data-ttu-id="d959c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d959c-110">Permission type</span></span> | <span data-ttu-id="d959c-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d959c-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="d959c-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d959c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d959c-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d959c-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="d959c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d959c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d959c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d959c-115">Not supported.</span></span> |
| <span data-ttu-id="d959c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d959c-116">Application</span></span> | <span data-ttu-id="d959c-117">Привилежедакцесс. Read. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="d959c-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="d959c-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="d959c-118">Azure AD</span></span>

| <span data-ttu-id="d959c-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d959c-119">Permission type</span></span> | <span data-ttu-id="d959c-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d959c-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="d959c-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d959c-121">Delegated (work or school account)</span></span> | <span data-ttu-id="d959c-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="d959c-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="d959c-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d959c-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d959c-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d959c-124">Not supported.</span></span> |
| <span data-ttu-id="d959c-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="d959c-125">Application</span></span> | <span data-ttu-id="d959c-126">Привилежедакцесс. Read. AzureAD</span><span class="sxs-lookup"><span data-stu-id="d959c-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="d959c-127">Группы</span><span class="sxs-lookup"><span data-stu-id="d959c-127">Groups</span></span>

|<span data-ttu-id="d959c-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d959c-128">Permission type</span></span> | <span data-ttu-id="d959c-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d959c-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="d959c-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d959c-130">Delegated (work or school account)</span></span> | <span data-ttu-id="d959c-131">Привилежедакцесс. ReadWrite. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="d959c-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="d959c-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d959c-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d959c-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d959c-133">Not supported.</span></span> |
| <span data-ttu-id="d959c-134">Приложение</span><span class="sxs-lookup"><span data-stu-id="d959c-134">Application</span></span> | <span data-ttu-id="d959c-135">Привилежедакцесс. Read. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="d959c-135">PrivilegedAccess.Read.AzureADGroups</span></span> |


## <a name="http-request"></a><span data-ttu-id="d959c-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d959c-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d959c-137">Экспорт коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) для ресурса</span><span class="sxs-lookup"><span data-stu-id="d959c-137">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="d959c-138">**Примечание:** Кроме области разрешений, этот запрос требует, чтобы запрашивающая сторона состроила по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="d959c-138">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="d959c-139">Экспорт коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="d959c-139">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d959c-140">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d959c-140">Optional query parameters</span></span>
<span data-ttu-id="d959c-141">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d959c-141">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d959c-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d959c-142">Request headers</span></span>
| <span data-ttu-id="d959c-143">Имя</span><span class="sxs-lookup"><span data-stu-id="d959c-143">Name</span></span>      |<span data-ttu-id="d959c-144">Описание</span><span class="sxs-lookup"><span data-stu-id="d959c-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d959c-145">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d959c-145">Authorization</span></span>  | <span data-ttu-id="d959c-146">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d959c-146">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d959c-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d959c-147">Request body</span></span>
<span data-ttu-id="d959c-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d959c-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d959c-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="d959c-149">Response</span></span>
<span data-ttu-id="d959c-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и содержимое типа `application/octet-stream` .</span><span class="sxs-lookup"><span data-stu-id="d959c-150">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="d959c-151">Пример</span><span class="sxs-lookup"><span data-stu-id="d959c-151">Example</span></span>
<span data-ttu-id="d959c-152">В этом примере все назначения ролей сохраняются в виде CSV-файла в подписке Wingtip Toys-произ.</span><span class="sxs-lookup"><span data-stu-id="d959c-152">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="d959c-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="d959c-153">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="d959c-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="d959c-154">Response</span></span>
<span data-ttu-id="d959c-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d959c-155">Here is an example of the response.</span></span> 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


