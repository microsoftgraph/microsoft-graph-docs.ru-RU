---
title: Создание Секуритибаселинестате
description: Создание нового объекта Секуритибаселинестате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a365d1e59696e89f6812490422722285f3645fc5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466079"
---
# <a name="create-securitybaselinestate"></a><span data-ttu-id="75f05-103">Создание Секуритибаселинестате</span><span class="sxs-lookup"><span data-stu-id="75f05-103">Create securityBaselineState</span></span>

> <span data-ttu-id="75f05-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75f05-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75f05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75f05-106">Создание нового объекта [секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md) .</span><span class="sxs-lookup"><span data-stu-id="75f05-106">Create a new [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75f05-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="75f05-107">Prerequisites</span></span>
<span data-ttu-id="75f05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75f05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75f05-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75f05-110">Permission type</span></span>|<span data-ttu-id="75f05-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75f05-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75f05-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75f05-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75f05-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75f05-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75f05-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75f05-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75f05-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f05-115">Not supported.</span></span>|
|<span data-ttu-id="75f05-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75f05-116">Application</span></span>|<span data-ttu-id="75f05-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f05-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75f05-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75f05-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates
```

## <a name="request-headers"></a><span data-ttu-id="75f05-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75f05-119">Request headers</span></span>
|<span data-ttu-id="75f05-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75f05-120">Header</span></span>|<span data-ttu-id="75f05-121">Значение</span><span class="sxs-lookup"><span data-stu-id="75f05-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75f05-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75f05-122">Authorization</span></span>|<span data-ttu-id="75f05-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75f05-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75f05-124">Accept</span><span class="sxs-lookup"><span data-stu-id="75f05-124">Accept</span></span>|<span data-ttu-id="75f05-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75f05-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75f05-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75f05-126">Request body</span></span>
<span data-ttu-id="75f05-127">В тексте запроса добавьте представление объекта Секуритибаселинестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75f05-127">In the request body, supply a JSON representation for the securityBaselineState object.</span></span>

<span data-ttu-id="75f05-128">В следующей таблице приведены свойства, необходимые при создании Секуритибаселинестате.</span><span class="sxs-lookup"><span data-stu-id="75f05-128">The following table shows the properties that are required when you create the securityBaselineState.</span></span>

|<span data-ttu-id="75f05-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="75f05-129">Property</span></span>|<span data-ttu-id="75f05-130">Тип</span><span class="sxs-lookup"><span data-stu-id="75f05-130">Type</span></span>|<span data-ttu-id="75f05-131">Описание</span><span class="sxs-lookup"><span data-stu-id="75f05-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75f05-132">id</span><span class="sxs-lookup"><span data-stu-id="75f05-132">id</span></span>|<span data-ttu-id="75f05-133">String</span><span class="sxs-lookup"><span data-stu-id="75f05-133">String</span></span>|<span data-ttu-id="75f05-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="75f05-134">Key of the entity.</span></span>|
|<span data-ttu-id="75f05-135">Секуритибаселинетемплатеид</span><span class="sxs-lookup"><span data-stu-id="75f05-135">securityBaselineTemplateId</span></span>|<span data-ttu-id="75f05-136">String</span><span class="sxs-lookup"><span data-stu-id="75f05-136">String</span></span>|<span data-ttu-id="75f05-137">Идентификатор шаблона базовой безопасности</span><span class="sxs-lookup"><span data-stu-id="75f05-137">The security baseline template id</span></span>|
|<span data-ttu-id="75f05-138">displayName</span><span class="sxs-lookup"><span data-stu-id="75f05-138">displayName</span></span>|<span data-ttu-id="75f05-139">String</span><span class="sxs-lookup"><span data-stu-id="75f05-139">String</span></span>|<span data-ttu-id="75f05-140">Отображаемое имя базового плана безопасности</span><span class="sxs-lookup"><span data-stu-id="75f05-140">The display name of the security baseline</span></span>|



## <a name="response"></a><span data-ttu-id="75f05-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="75f05-141">Response</span></span>
<span data-ttu-id="75f05-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75f05-142">If successful, this method returns a `201 Created` response code and a [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75f05-143">Пример</span><span class="sxs-lookup"><span data-stu-id="75f05-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="75f05-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="75f05-144">Request</span></span>
<span data-ttu-id="75f05-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75f05-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates
Content-type: application/json
Content-length: 175

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="75f05-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="75f05-146">Response</span></span>
<span data-ttu-id="75f05-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75f05-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 224

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "23dc2503-2503-23dc-0325-dc230325dc23",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```



