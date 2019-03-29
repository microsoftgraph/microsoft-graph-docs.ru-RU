---
title: Удаление объекта deviceComplianceSettingState
description: Удаляет объект deviceComplianceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc06210fdee3bf6dc1d675eb34594ceca06e8339
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976479"
---
# <a name="delete-devicecompliancesettingstate"></a><span data-ttu-id="c3422-103">Удаление объекта deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="c3422-103">Delete deviceComplianceSettingState</span></span>

> <span data-ttu-id="c3422-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3422-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3422-105">Удаляет объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="c3422-105">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3422-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c3422-106">Prerequisites</span></span>
<span data-ttu-id="c3422-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3422-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3422-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3422-109">Permission type</span></span>|<span data-ttu-id="c3422-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3422-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3422-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3422-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3422-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3422-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3422-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3422-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3422-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3422-114">Not supported.</span></span>|
|<span data-ttu-id="c3422-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3422-115">Application</span></span>|<span data-ttu-id="c3422-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3422-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3422-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3422-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c3422-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3422-118">Request headers</span></span>
|<span data-ttu-id="c3422-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3422-119">Header</span></span>|<span data-ttu-id="c3422-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c3422-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3422-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3422-121">Authorization</span></span>|<span data-ttu-id="c3422-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3422-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3422-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c3422-123">Accept</span></span>|<span data-ttu-id="c3422-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c3422-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3422-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3422-125">Request body</span></span>
<span data-ttu-id="c3422-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3422-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3422-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3422-127">Response</span></span>
<span data-ttu-id="c3422-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c3422-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c3422-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c3422-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3422-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3422-130">Request</span></span>
<span data-ttu-id="c3422-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3422-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="c3422-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3422-132">Response</span></span>
<span data-ttu-id="c3422-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3422-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



