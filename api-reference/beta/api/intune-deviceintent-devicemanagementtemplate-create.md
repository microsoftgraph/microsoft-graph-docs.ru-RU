---
title: Создание Девицеманажементтемплате
description: Создание нового объекта Девицеманажементтемплате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23c86d654d229c4932a9e5b7d86d980416637b2a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466583"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="28606-103">Создание Девицеманажементтемплате</span><span class="sxs-lookup"><span data-stu-id="28606-103">Create deviceManagementTemplate</span></span>

> <span data-ttu-id="28606-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28606-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28606-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28606-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28606-106">Создание нового объекта [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="28606-106">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28606-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="28606-107">Prerequisites</span></span>
<span data-ttu-id="28606-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28606-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28606-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28606-110">Permission type</span></span>|<span data-ttu-id="28606-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="28606-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28606-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28606-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28606-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28606-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28606-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28606-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28606-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28606-115">Not supported.</span></span>|
|<span data-ttu-id="28606-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28606-116">Application</span></span>|<span data-ttu-id="28606-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28606-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28606-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28606-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
```

## <a name="request-headers"></a><span data-ttu-id="28606-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28606-119">Request headers</span></span>
|<span data-ttu-id="28606-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28606-120">Header</span></span>|<span data-ttu-id="28606-121">Значение</span><span class="sxs-lookup"><span data-stu-id="28606-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28606-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28606-122">Authorization</span></span>|<span data-ttu-id="28606-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28606-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28606-124">Accept</span><span class="sxs-lookup"><span data-stu-id="28606-124">Accept</span></span>|<span data-ttu-id="28606-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28606-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28606-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28606-126">Request body</span></span>
<span data-ttu-id="28606-127">В тексте запроса добавьте представление объекта Девицеманажементтемплате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28606-127">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="28606-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементтемплате.</span><span class="sxs-lookup"><span data-stu-id="28606-128">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="28606-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="28606-129">Property</span></span>|<span data-ttu-id="28606-130">Тип</span><span class="sxs-lookup"><span data-stu-id="28606-130">Type</span></span>|<span data-ttu-id="28606-131">Описание</span><span class="sxs-lookup"><span data-stu-id="28606-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28606-132">id</span><span class="sxs-lookup"><span data-stu-id="28606-132">id</span></span>|<span data-ttu-id="28606-133">Строка</span><span class="sxs-lookup"><span data-stu-id="28606-133">String</span></span>|<span data-ttu-id="28606-134">Идентификатор шаблона</span><span class="sxs-lookup"><span data-stu-id="28606-134">The template ID</span></span>|
|<span data-ttu-id="28606-135">displayName</span><span class="sxs-lookup"><span data-stu-id="28606-135">displayName</span></span>|<span data-ttu-id="28606-136">String</span><span class="sxs-lookup"><span data-stu-id="28606-136">String</span></span>|<span data-ttu-id="28606-137">Отображаемое имя шаблона</span><span class="sxs-lookup"><span data-stu-id="28606-137">The template's display name</span></span>|
|<span data-ttu-id="28606-138">description</span><span class="sxs-lookup"><span data-stu-id="28606-138">description</span></span>|<span data-ttu-id="28606-139">String</span><span class="sxs-lookup"><span data-stu-id="28606-139">String</span></span>|<span data-ttu-id="28606-140">Описание шаблона</span><span class="sxs-lookup"><span data-stu-id="28606-140">The template's description</span></span>|



## <a name="response"></a><span data-ttu-id="28606-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="28606-141">Response</span></span>
<span data-ttu-id="28606-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28606-142">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28606-143">Пример</span><span class="sxs-lookup"><span data-stu-id="28606-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="28606-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="28606-144">Request</span></span>
<span data-ttu-id="28606-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28606-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="28606-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="28606-146">Response</span></span>
<span data-ttu-id="28606-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28606-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 194

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
  "displayName": "Display Name value",
  "description": "Description value"
}
```





