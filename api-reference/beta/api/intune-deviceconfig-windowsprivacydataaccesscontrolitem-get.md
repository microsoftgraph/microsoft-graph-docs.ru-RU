---
title: Получение Виндовспривацидатаакцессконтролитем
description: Чтение свойств и связей объекта Виндовспривацидатаакцессконтролитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bcd8d3c15a64532c31a8b258c90a40f540557e31
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961387"
---
# <a name="get-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="89281-103">Получение Виндовспривацидатаакцессконтролитем</span><span class="sxs-lookup"><span data-stu-id="89281-103">Get windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="89281-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89281-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89281-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89281-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89281-106">Чтение свойств и связей объекта [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="89281-106">Read properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89281-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="89281-107">Prerequisites</span></span>
<span data-ttu-id="89281-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89281-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89281-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89281-110">Permission type</span></span>|<span data-ttu-id="89281-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89281-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89281-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89281-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89281-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89281-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="89281-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89281-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89281-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89281-115">Not supported.</span></span>|
|<span data-ttu-id="89281-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89281-116">Application</span></span>|<span data-ttu-id="89281-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89281-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89281-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89281-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89281-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="89281-119">Optional query parameters</span></span>
<span data-ttu-id="89281-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="89281-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89281-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89281-121">Request headers</span></span>
|<span data-ttu-id="89281-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89281-122">Header</span></span>|<span data-ttu-id="89281-123">Значение</span><span class="sxs-lookup"><span data-stu-id="89281-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89281-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89281-124">Authorization</span></span>|<span data-ttu-id="89281-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89281-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89281-126">Accept</span><span class="sxs-lookup"><span data-stu-id="89281-126">Accept</span></span>|<span data-ttu-id="89281-127">application/json</span><span class="sxs-lookup"><span data-stu-id="89281-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89281-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="89281-128">Request body</span></span>
<span data-ttu-id="89281-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89281-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89281-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="89281-130">Response</span></span>
<span data-ttu-id="89281-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89281-131">If successful, this method returns a `200 OK` response code and [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89281-132">Пример</span><span class="sxs-lookup"><span data-stu-id="89281-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="89281-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="89281-133">Request</span></span>
<span data-ttu-id="89281-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89281-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

### <a name="response"></a><span data-ttu-id="89281-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="89281-135">Response</span></span>
<span data-ttu-id="89281-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89281-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
    "id": "03b15556-5556-03b1-5655-b1035655b103",
    "accessLevel": "forceAllow",
    "dataCategory": "accountInfo",
    "appPackageFamilyName": "App Package Family Name value",
    "appDisplayName": "App Display Name value"
  }
}
```





