---
title: Список windowsPrivacyDataAccessControlItems
description: Свойства списка и связей объектов windowsPrivacyDataAccessControlItem.
author: tfitzmac
ms.openlocfilehash: 642db3e0381adf3bedfff52baf4987b7ea43cdaf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303173"
---
# <a name="list-windowsprivacydataaccesscontrolitems"></a><span data-ttu-id="c5692-103">Список windowsPrivacyDataAccessControlItems</span><span class="sxs-lookup"><span data-stu-id="c5692-103">List windowsPrivacyDataAccessControlItems</span></span>

> <span data-ttu-id="c5692-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5692-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5692-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5692-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5692-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c5692-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5692-107">Свойства списка и связей объектов [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="c5692-107">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5692-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5692-108">Prerequisites</span></span>
<span data-ttu-id="c5692-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5692-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5692-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5692-111">Permission type</span></span>|<span data-ttu-id="c5692-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5692-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5692-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5692-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5692-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5692-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c5692-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5692-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5692-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5692-116">Not supported.</span></span>|
|<span data-ttu-id="c5692-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5692-117">Application</span></span>|<span data-ttu-id="c5692-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5692-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5692-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5692-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="c5692-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5692-120">Request headers</span></span>
|<span data-ttu-id="c5692-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5692-121">Header</span></span>|<span data-ttu-id="c5692-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c5692-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5692-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5692-123">Authorization</span></span>|<span data-ttu-id="c5692-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c5692-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5692-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5692-125">Accept</span></span>|<span data-ttu-id="c5692-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5692-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5692-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5692-127">Request body</span></span>
<span data-ttu-id="c5692-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5692-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5692-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5692-129">Response</span></span>
<span data-ttu-id="c5692-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c5692-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5692-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c5692-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5692-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5692-132">Request</span></span>
<span data-ttu-id="c5692-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5692-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

### <a name="response"></a><span data-ttu-id="c5692-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5692-134">Response</span></span>
<span data-ttu-id="c5692-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c5692-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
      "id": "03b15556-5556-03b1-5655-b1035655b103",
      "accessLevel": "forceAllow",
      "dataCategory": "accountInfo",
      "appPackageFamilyName": "App Package Family Name value",
      "appDisplayName": "App Display Name value"
    }
  ]
}
```





