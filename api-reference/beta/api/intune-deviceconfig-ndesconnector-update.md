---
title: Обновление ndesConnector
description: Обновление свойства объекта ndesConnector.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8c78502bb0670eca08b896bf1a0b732f94b669cd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418423"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="4421a-103">Обновление ndesConnector</span><span class="sxs-lookup"><span data-stu-id="4421a-103">Update ndesConnector</span></span>

> <span data-ttu-id="4421a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4421a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4421a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4421a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4421a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4421a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4421a-107">Обновление свойства объекта [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="4421a-107">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4421a-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="4421a-108">Prerequisites</span></span>
<span data-ttu-id="4421a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4421a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4421a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4421a-111">Permission type</span></span>|<span data-ttu-id="4421a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4421a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4421a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4421a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4421a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4421a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4421a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4421a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4421a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4421a-116">Not supported.</span></span>|
|<span data-ttu-id="4421a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4421a-117">Application</span></span>|<span data-ttu-id="4421a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4421a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4421a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4421a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="4421a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4421a-120">Request headers</span></span>
|<span data-ttu-id="4421a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4421a-121">Header</span></span>|<span data-ttu-id="4421a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4421a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4421a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4421a-123">Authorization</span></span>|<span data-ttu-id="4421a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4421a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4421a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4421a-125">Accept</span></span>|<span data-ttu-id="4421a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4421a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4421a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4421a-127">Request body</span></span>
<span data-ttu-id="4421a-128">В тексте запроса укажите представление JSON для объекта [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="4421a-128">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="4421a-129">В следующей таблице показаны свойства, которые необходимы для создания [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span><span class="sxs-lookup"><span data-stu-id="4421a-129">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="4421a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4421a-130">Property</span></span>|<span data-ttu-id="4421a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4421a-131">Type</span></span>|<span data-ttu-id="4421a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4421a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4421a-133">id</span><span class="sxs-lookup"><span data-stu-id="4421a-133">id</span></span>|<span data-ttu-id="4421a-134">String</span><span class="sxs-lookup"><span data-stu-id="4421a-134">String</span></span>|<span data-ttu-id="4421a-135">Ключ NDES соединителя.</span><span class="sxs-lookup"><span data-stu-id="4421a-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="4421a-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="4421a-136">lastConnectionDateTime</span></span>|<span data-ttu-id="4421a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4421a-137">DateTimeOffset</span></span>|<span data-ttu-id="4421a-138">Время последнего подключения для соединителя Ndes</span><span class="sxs-lookup"><span data-stu-id="4421a-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="4421a-139">state</span><span class="sxs-lookup"><span data-stu-id="4421a-139">state</span></span>|[<span data-ttu-id="4421a-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="4421a-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="4421a-141">Состояние NDES соединителя.</span><span class="sxs-lookup"><span data-stu-id="4421a-141">Ndes Connector Status.</span></span> <span data-ttu-id="4421a-142">Возможные значения: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="4421a-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="4421a-143">displayName</span><span class="sxs-lookup"><span data-stu-id="4421a-143">displayName</span></span>|<span data-ttu-id="4421a-144">String</span><span class="sxs-lookup"><span data-stu-id="4421a-144">String</span></span>|<span data-ttu-id="4421a-145">Понятное имя соединителя Ndes.</span><span class="sxs-lookup"><span data-stu-id="4421a-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="4421a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4421a-146">Response</span></span>
<span data-ttu-id="4421a-147">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4421a-147">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4421a-148">Пример</span><span class="sxs-lookup"><span data-stu-id="4421a-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="4421a-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="4421a-149">Request</span></span>
<span data-ttu-id="4421a-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4421a-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="4421a-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="4421a-151">Response</span></span>
<span data-ttu-id="4421a-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4421a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```




