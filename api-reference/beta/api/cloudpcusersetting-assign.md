---
title: 'cloudPcUserSetting: назначение'
description: Назначение параметров пользователя облачного КОМПЬЮТЕРА группам пользователей.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 987ecf4ee31b2ade7baf08246542b13d14a3a6da
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993694"
---
# <a name="cloudpcusersetting-assign"></a><span data-ttu-id="5bd15-103">cloudPcUserSetting: назначение</span><span class="sxs-lookup"><span data-stu-id="5bd15-103">cloudPcUserSetting: assign</span></span>

<span data-ttu-id="5bd15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bd15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bd15-105">Назначение [cloudPcUserSetting группам](../resources/cloudpcusersetting.md) пользователей.</span><span class="sxs-lookup"><span data-stu-id="5bd15-105">Assign a [cloudPcUserSetting](../resources/cloudpcusersetting.md) to user groups.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="5bd15-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5bd15-106">Permissions</span></span>

<span data-ttu-id="5bd15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bd15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bd15-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bd15-109">Permission type</span></span>|<span data-ttu-id="5bd15-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bd15-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bd15-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bd15-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5bd15-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bd15-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="5bd15-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bd15-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bd15-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bd15-114">Not supported.</span></span>|
|<span data-ttu-id="5bd15-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5bd15-115">Application</span></span>|<span data-ttu-id="5bd15-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bd15-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bd15-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bd15-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/userSettings/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="5bd15-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bd15-118">Request headers</span></span>

|<span data-ttu-id="5bd15-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5bd15-119">Name</span></span>|<span data-ttu-id="5bd15-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5bd15-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5bd15-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5bd15-121">Authorization</span></span>|<span data-ttu-id="5bd15-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bd15-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5bd15-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5bd15-124">Content-Type</span></span>|<span data-ttu-id="5bd15-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bd15-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bd15-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5bd15-127">Request body</span></span>

<span data-ttu-id="5bd15-128">В корпусе запроса поставляем представление JSON объекта [cloudPcUserSettingAssignment.](../resources/cloudpcusersettingassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5bd15-128">In the request body, supply a JSON representation of the [cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) object.</span></span>

<span data-ttu-id="5bd15-129">В следующей таблице показаны свойства, необходимые при создании [cloudPcUserSettingAssignment.](../resources/cloudpcusersettingassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5bd15-129">The following table shows the properties that are required when you create the [cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md).</span></span>

|<span data-ttu-id="5bd15-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5bd15-130">Property</span></span>|<span data-ttu-id="5bd15-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5bd15-131">Type</span></span>|<span data-ttu-id="5bd15-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5bd15-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bd15-133">target</span><span class="sxs-lookup"><span data-stu-id="5bd15-133">target</span></span>|[<span data-ttu-id="5bd15-134">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5bd15-134">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="5bd15-135">Цель назначения для политики обеспечения.</span><span class="sxs-lookup"><span data-stu-id="5bd15-135">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="5bd15-136">В настоящее время единственной поддерживаемой целевой группой является группа пользователей.</span><span class="sxs-lookup"><span data-stu-id="5bd15-136">Currently, the only target supported is a user group.</span></span>|

## <a name="response"></a><span data-ttu-id="5bd15-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bd15-137">Response</span></span>

<span data-ttu-id="5bd15-138">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5bd15-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5bd15-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="5bd15-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5bd15-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bd15-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "cloudpcusersetting_assign"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff/assign
Content-Type: application/json
Content-length: 254

{
  "assignments": [
    {
      "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
      "target":{
        "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
        "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
        }
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="5bd15-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bd15-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
