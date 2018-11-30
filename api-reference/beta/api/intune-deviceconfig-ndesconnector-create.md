---
title: Создание ndesConnector
description: Создание нового объекта ndesConnector.
ms.openlocfilehash: 0dd1ee403a03d72e5bd9c0dd8febcfb28a01a36e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078041"
---
# <a name="create-ndesconnector"></a><span data-ttu-id="f9fed-103">Создание ndesConnector</span><span class="sxs-lookup"><span data-stu-id="f9fed-103">Create ndesConnector</span></span>

> <span data-ttu-id="f9fed-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f9fed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9fed-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9fed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9fed-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f9fed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9fed-107">Создание нового объекта [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="f9fed-107">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9fed-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f9fed-108">Prerequisites</span></span>
<span data-ttu-id="f9fed-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9fed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9fed-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9fed-111">Permission type</span></span>|<span data-ttu-id="f9fed-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9fed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9fed-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9fed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9fed-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9fed-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9fed-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9fed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9fed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9fed-116">Not supported.</span></span>|
|<span data-ttu-id="f9fed-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9fed-117">Application</span></span>|<span data-ttu-id="f9fed-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9fed-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9fed-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9fed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="f9fed-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9fed-120">Request headers</span></span>
|<span data-ttu-id="f9fed-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9fed-121">Header</span></span>|<span data-ttu-id="f9fed-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f9fed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9fed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9fed-123">Authorization</span></span>|<span data-ttu-id="f9fed-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f9fed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9fed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f9fed-125">Accept</span></span>|<span data-ttu-id="f9fed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9fed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9fed-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9fed-127">Request body</span></span>
<span data-ttu-id="f9fed-128">В тексте запроса укажите представление JSON для объекта ndesConnector.</span><span class="sxs-lookup"><span data-stu-id="f9fed-128">In the request body, supply a JSON representation for the ndesConnector object.</span></span>

<span data-ttu-id="f9fed-129">В следующей таблице показаны свойства, которые необходимы для создания ndesConnector.</span><span class="sxs-lookup"><span data-stu-id="f9fed-129">The following table shows the properties that are required when you create the ndesConnector.</span></span>

|<span data-ttu-id="f9fed-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9fed-130">Property</span></span>|<span data-ttu-id="f9fed-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f9fed-131">Type</span></span>|<span data-ttu-id="f9fed-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f9fed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9fed-133">id</span><span class="sxs-lookup"><span data-stu-id="f9fed-133">id</span></span>|<span data-ttu-id="f9fed-134">String</span><span class="sxs-lookup"><span data-stu-id="f9fed-134">String</span></span>|<span data-ttu-id="f9fed-135">Ключ NDES соединителя.</span><span class="sxs-lookup"><span data-stu-id="f9fed-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="f9fed-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="f9fed-136">lastConnectionDateTime</span></span>|<span data-ttu-id="f9fed-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9fed-137">DateTimeOffset</span></span>|<span data-ttu-id="f9fed-138">Время последнего подключения для соединителя Ndes</span><span class="sxs-lookup"><span data-stu-id="f9fed-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="f9fed-139">state</span><span class="sxs-lookup"><span data-stu-id="f9fed-139">state</span></span>|[<span data-ttu-id="f9fed-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="f9fed-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="f9fed-141">Состояние NDES соединителя.</span><span class="sxs-lookup"><span data-stu-id="f9fed-141">Ndes Connector Status.</span></span> <span data-ttu-id="f9fed-142">Возможные значения: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="f9fed-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="f9fed-143">displayName</span><span class="sxs-lookup"><span data-stu-id="f9fed-143">displayName</span></span>|<span data-ttu-id="f9fed-144">String</span><span class="sxs-lookup"><span data-stu-id="f9fed-144">String</span></span>|<span data-ttu-id="f9fed-145">Понятное имя соединителя Ndes.</span><span class="sxs-lookup"><span data-stu-id="f9fed-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="f9fed-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9fed-146">Response</span></span>
<span data-ttu-id="f9fed-147">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f9fed-147">If successful, this method returns a `201 Created` response code and a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9fed-148">Пример</span><span class="sxs-lookup"><span data-stu-id="f9fed-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9fed-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9fed-149">Request</span></span>
<span data-ttu-id="f9fed-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9fed-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9fed-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9fed-151">Response</span></span>
<span data-ttu-id="f9fed-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f9fed-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





