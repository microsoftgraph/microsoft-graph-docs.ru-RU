---
title: Обновление Секуритибаселинестате
description: Обновление свойств объекта Секуритибаселинестате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 33f4a65937f8139aa7ebee483cad6e66f989caa0
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522848"
---
# <a name="update-securitybaselinestate"></a><span data-ttu-id="4f0ca-103">Обновление Секуритибаселинестате</span><span class="sxs-lookup"><span data-stu-id="4f0ca-103">Update securityBaselineState</span></span>

> <span data-ttu-id="4f0ca-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f0ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f0ca-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f0ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f0ca-106">Обновление свойств объекта [секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md) .</span><span class="sxs-lookup"><span data-stu-id="4f0ca-106">Update the properties of a [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f0ca-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4f0ca-107">Prerequisites</span></span>
<span data-ttu-id="4f0ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4f0ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4f0ca-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f0ca-110">Permission type</span></span>|<span data-ttu-id="4f0ca-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f0ca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f0ca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f0ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f0ca-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f0ca-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f0ca-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f0ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f0ca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f0ca-115">Not supported.</span></span>|
|<span data-ttu-id="4f0ca-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f0ca-116">Application</span></span>|<span data-ttu-id="4f0ca-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f0ca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f0ca-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f0ca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}
```

## <a name="request-headers"></a><span data-ttu-id="4f0ca-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f0ca-119">Request headers</span></span>
|<span data-ttu-id="4f0ca-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f0ca-120">Header</span></span>|<span data-ttu-id="4f0ca-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4f0ca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f0ca-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f0ca-122">Authorization</span></span>|<span data-ttu-id="4f0ca-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f0ca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f0ca-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4f0ca-124">Accept</span></span>|<span data-ttu-id="4f0ca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f0ca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f0ca-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f0ca-126">Request body</span></span>
<span data-ttu-id="4f0ca-127">В тексте запроса добавьте представление объекта [Секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f0ca-127">In the request body, supply a JSON representation for the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

<span data-ttu-id="4f0ca-128">В следующей таблице приведены свойства, необходимые при создании [секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md).</span><span class="sxs-lookup"><span data-stu-id="4f0ca-128">The following table shows the properties that are required when you create the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md).</span></span>

|<span data-ttu-id="4f0ca-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f0ca-129">Property</span></span>|<span data-ttu-id="4f0ca-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4f0ca-130">Type</span></span>|<span data-ttu-id="4f0ca-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4f0ca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f0ca-132">id</span><span class="sxs-lookup"><span data-stu-id="4f0ca-132">id</span></span>|<span data-ttu-id="4f0ca-133">String</span><span class="sxs-lookup"><span data-stu-id="4f0ca-133">String</span></span>|<span data-ttu-id="4f0ca-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4f0ca-134">Key of the entity.</span></span>|
|<span data-ttu-id="4f0ca-135">Секуритибаселинетемплатеид</span><span class="sxs-lookup"><span data-stu-id="4f0ca-135">securityBaselineTemplateId</span></span>|<span data-ttu-id="4f0ca-136">String</span><span class="sxs-lookup"><span data-stu-id="4f0ca-136">String</span></span>|<span data-ttu-id="4f0ca-137">Идентификатор шаблона базовой безопасности</span><span class="sxs-lookup"><span data-stu-id="4f0ca-137">The security baseline template id</span></span>|
|<span data-ttu-id="4f0ca-138">displayName</span><span class="sxs-lookup"><span data-stu-id="4f0ca-138">displayName</span></span>|<span data-ttu-id="4f0ca-139">String</span><span class="sxs-lookup"><span data-stu-id="4f0ca-139">String</span></span>|<span data-ttu-id="4f0ca-140">Отображаемое имя базового плана безопасности</span><span class="sxs-lookup"><span data-stu-id="4f0ca-140">The display name of the security baseline</span></span>|



## <a name="response"></a><span data-ttu-id="4f0ca-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f0ca-141">Response</span></span>
<span data-ttu-id="4f0ca-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4f0ca-142">If successful, this method returns a `200 OK` response code and an updated [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f0ca-143">Пример</span><span class="sxs-lookup"><span data-stu-id="4f0ca-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f0ca-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f0ca-144">Request</span></span>
<span data-ttu-id="4f0ca-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f0ca-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}
Content-type: application/json
Content-length: 175

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="4f0ca-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f0ca-146">Response</span></span>
<span data-ttu-id="4f0ca-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f0ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 224

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "23dc2503-2503-23dc-0325-dc230325dc23",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```



