---
title: Создание ndesConnector
description: Создание нового объекта ndesConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 809a324665136927796790e88d3beb742cf06be4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940185"
---
# <a name="create-ndesconnector"></a><span data-ttu-id="19fbf-103">Создание ndesConnector</span><span class="sxs-lookup"><span data-stu-id="19fbf-103">Create ndesConnector</span></span>

> <span data-ttu-id="19fbf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="19fbf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19fbf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19fbf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19fbf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="19fbf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19fbf-107">Создание нового объекта [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="19fbf-107">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="19fbf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="19fbf-108">Prerequisites</span></span>
<span data-ttu-id="19fbf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19fbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19fbf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19fbf-111">Permission type</span></span>|<span data-ttu-id="19fbf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19fbf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19fbf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19fbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19fbf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19fbf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19fbf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19fbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19fbf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19fbf-116">Not supported.</span></span>|
|<span data-ttu-id="19fbf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19fbf-117">Application</span></span>|<span data-ttu-id="19fbf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19fbf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19fbf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19fbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="19fbf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19fbf-120">Request headers</span></span>
|<span data-ttu-id="19fbf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19fbf-121">Header</span></span>|<span data-ttu-id="19fbf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="19fbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19fbf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19fbf-123">Authorization</span></span>|<span data-ttu-id="19fbf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="19fbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19fbf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="19fbf-125">Accept</span></span>|<span data-ttu-id="19fbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19fbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19fbf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19fbf-127">Request body</span></span>
<span data-ttu-id="19fbf-128">В тексте запроса укажите представление JSON для объекта ndesConnector.</span><span class="sxs-lookup"><span data-stu-id="19fbf-128">In the request body, supply a JSON representation for the ndesConnector object.</span></span>

<span data-ttu-id="19fbf-129">В следующей таблице показаны свойства, которые необходимы для создания ndesConnector.</span><span class="sxs-lookup"><span data-stu-id="19fbf-129">The following table shows the properties that are required when you create the ndesConnector.</span></span>

|<span data-ttu-id="19fbf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="19fbf-130">Property</span></span>|<span data-ttu-id="19fbf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="19fbf-131">Type</span></span>|<span data-ttu-id="19fbf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="19fbf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19fbf-133">id</span><span class="sxs-lookup"><span data-stu-id="19fbf-133">id</span></span>|<span data-ttu-id="19fbf-134">Строка</span><span class="sxs-lookup"><span data-stu-id="19fbf-134">String</span></span>|<span data-ttu-id="19fbf-135">Ключ NDES соединителя.</span><span class="sxs-lookup"><span data-stu-id="19fbf-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="19fbf-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="19fbf-136">lastConnectionDateTime</span></span>|<span data-ttu-id="19fbf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19fbf-137">DateTimeOffset</span></span>|<span data-ttu-id="19fbf-138">Время последнего подключения для соединителя Ndes</span><span class="sxs-lookup"><span data-stu-id="19fbf-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="19fbf-139">state</span><span class="sxs-lookup"><span data-stu-id="19fbf-139">state</span></span>|[<span data-ttu-id="19fbf-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="19fbf-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="19fbf-141">Состояние NDES соединителя.</span><span class="sxs-lookup"><span data-stu-id="19fbf-141">Ndes Connector Status.</span></span> <span data-ttu-id="19fbf-142">Возможные значения: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="19fbf-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="19fbf-143">displayName</span><span class="sxs-lookup"><span data-stu-id="19fbf-143">displayName</span></span>|<span data-ttu-id="19fbf-144">Строка</span><span class="sxs-lookup"><span data-stu-id="19fbf-144">String</span></span>|<span data-ttu-id="19fbf-145">Понятное имя соединителя Ndes.</span><span class="sxs-lookup"><span data-stu-id="19fbf-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="19fbf-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="19fbf-146">Response</span></span>
<span data-ttu-id="19fbf-147">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="19fbf-147">If successful, this method returns a `201 Created` response code and a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19fbf-148">Пример</span><span class="sxs-lookup"><span data-stu-id="19fbf-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="19fbf-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="19fbf-149">Request</span></span>
<span data-ttu-id="19fbf-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19fbf-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/ndesConnectors
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="19fbf-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="19fbf-151">Response</span></span>
<span data-ttu-id="19fbf-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="19fbf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





