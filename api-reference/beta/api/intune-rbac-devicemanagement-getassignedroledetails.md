---
title: Функция Жетассигнедроледетаилс
description: Извлекает назначенные определения ролей и назначения ролей для текущего пользователя, прошедшего проверку подлинности.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f3b3f843fe521e0a9cc94fa33ba94a4f76a3514
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002275"
---
# <a name="getassignedroledetails-function"></a><span data-ttu-id="c0388-103">Функция Жетассигнедроледетаилс</span><span class="sxs-lookup"><span data-stu-id="c0388-103">getAssignedRoleDetails function</span></span>

> <span data-ttu-id="c0388-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0388-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0388-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0388-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0388-106">Извлекает назначенные определения ролей и назначения ролей для текущего пользователя, прошедшего проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="c0388-106">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0388-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c0388-107">Prerequisites</span></span>
<span data-ttu-id="c0388-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0388-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0388-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0388-110">Permission type</span></span>|<span data-ttu-id="c0388-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0388-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0388-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0388-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0388-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0388-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="c0388-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0388-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0388-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0388-115">Not supported.</span></span>|
|<span data-ttu-id="c0388-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0388-116">Application</span></span>|<span data-ttu-id="c0388-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0388-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0388-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0388-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleDetails
```

## <a name="request-headers"></a><span data-ttu-id="c0388-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0388-119">Request headers</span></span>
|<span data-ttu-id="c0388-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0388-120">Header</span></span>|<span data-ttu-id="c0388-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c0388-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0388-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0388-122">Authorization</span></span>|<span data-ttu-id="c0388-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0388-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0388-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c0388-124">Accept</span></span>|<span data-ttu-id="c0388-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0388-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0388-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c0388-126">Request body</span></span>
<span data-ttu-id="c0388-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0388-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0388-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0388-128">Response</span></span>
<span data-ttu-id="c0388-129">В случае успеха эта функция возвращает код `200 OK` отклика и объект [девицеандаппманажементассигнедроледетаилс](../resources/intune-rbac-deviceandappmanagementassignedroledetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0388-129">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementAssignedRoleDetails](../resources/intune-rbac-deviceandappmanagementassignedroledetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0388-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c0388-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0388-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0388-131">Request</span></span>
<span data-ttu-id="c0388-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0388-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleDetails
```

### <a name="response"></a><span data-ttu-id="c0388-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0388-133">Response</span></span>
<span data-ttu-id="c0388-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0388-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 245

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
    "roleDefinitionIds": [
      "Role Definition Ids value"
    ],
    "roleAssignmentIds": [
      "Role Assignment Ids value"
    ]
  }
}
```





