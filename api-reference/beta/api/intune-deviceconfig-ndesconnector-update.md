---
title: Обновление ndesConnector
description: Обновление свойства объекта ndesConnector.
author: tfitzmac
ms.openlocfilehash: 80a518a403ce2354ec2f0a633520baf98ae2c7c3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358305"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="48dcc-103">Обновление ndesConnector</span><span class="sxs-lookup"><span data-stu-id="48dcc-103">Update ndesConnector</span></span>

> <span data-ttu-id="48dcc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="48dcc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48dcc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48dcc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48dcc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="48dcc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48dcc-107">Обновление свойства объекта [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="48dcc-107">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="48dcc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="48dcc-108">Prerequisites</span></span>
<span data-ttu-id="48dcc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48dcc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48dcc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48dcc-111">Permission type</span></span>|<span data-ttu-id="48dcc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48dcc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48dcc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48dcc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48dcc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48dcc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="48dcc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48dcc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48dcc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48dcc-116">Not supported.</span></span>|
|<span data-ttu-id="48dcc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48dcc-117">Application</span></span>|<span data-ttu-id="48dcc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48dcc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48dcc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48dcc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="48dcc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48dcc-120">Request headers</span></span>
|<span data-ttu-id="48dcc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48dcc-121">Header</span></span>|<span data-ttu-id="48dcc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="48dcc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48dcc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48dcc-123">Authorization</span></span>|<span data-ttu-id="48dcc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="48dcc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48dcc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="48dcc-125">Accept</span></span>|<span data-ttu-id="48dcc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48dcc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48dcc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48dcc-127">Request body</span></span>
<span data-ttu-id="48dcc-128">В тексте запроса укажите представление JSON для объекта [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="48dcc-128">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="48dcc-129">В следующей таблице показаны свойства, которые необходимы для создания [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span><span class="sxs-lookup"><span data-stu-id="48dcc-129">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="48dcc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="48dcc-130">Property</span></span>|<span data-ttu-id="48dcc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="48dcc-131">Type</span></span>|<span data-ttu-id="48dcc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="48dcc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48dcc-133">id</span><span class="sxs-lookup"><span data-stu-id="48dcc-133">id</span></span>|<span data-ttu-id="48dcc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="48dcc-134">String</span></span>|<span data-ttu-id="48dcc-135">Ключ NDES соединителя.</span><span class="sxs-lookup"><span data-stu-id="48dcc-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="48dcc-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="48dcc-136">lastConnectionDateTime</span></span>|<span data-ttu-id="48dcc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48dcc-137">DateTimeOffset</span></span>|<span data-ttu-id="48dcc-138">Время последнего подключения для соединителя Ndes</span><span class="sxs-lookup"><span data-stu-id="48dcc-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="48dcc-139">state</span><span class="sxs-lookup"><span data-stu-id="48dcc-139">state</span></span>|[<span data-ttu-id="48dcc-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="48dcc-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="48dcc-141">Состояние NDES соединителя.</span><span class="sxs-lookup"><span data-stu-id="48dcc-141">Ndes Connector Status.</span></span> <span data-ttu-id="48dcc-142">Возможные значения: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="48dcc-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="48dcc-143">displayName</span><span class="sxs-lookup"><span data-stu-id="48dcc-143">displayName</span></span>|<span data-ttu-id="48dcc-144">Строка</span><span class="sxs-lookup"><span data-stu-id="48dcc-144">String</span></span>|<span data-ttu-id="48dcc-145">Понятное имя соединителя Ndes.</span><span class="sxs-lookup"><span data-stu-id="48dcc-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="48dcc-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="48dcc-146">Response</span></span>
<span data-ttu-id="48dcc-147">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="48dcc-147">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48dcc-148">Пример</span><span class="sxs-lookup"><span data-stu-id="48dcc-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="48dcc-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="48dcc-149">Request</span></span>
<span data-ttu-id="48dcc-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48dcc-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
Content-type: application/json
Content-length: 131

{
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="48dcc-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="48dcc-151">Response</span></span>
<span data-ttu-id="48dcc-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="48dcc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





