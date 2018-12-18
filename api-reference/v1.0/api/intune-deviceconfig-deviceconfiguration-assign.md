---
title: Действие assign
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 4a7eea2b7fe321536add6dcbe458d1b3d7ec6e88
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355400"
---
# <a name="assign-action"></a><span data-ttu-id="b6a5d-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="b6a5d-103">assign action</span></span>

> <span data-ttu-id="b6a5d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b6a5d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6a5d-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b6a5d-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6a5d-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a5d-106">Prerequisites</span></span>
<span data-ttu-id="b6a5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6a5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6a5d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a5d-109">Permission type</span></span>|<span data-ttu-id="b6a5d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6a5d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6a5d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6a5d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b6a5d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6a5d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6a5d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6a5d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6a5d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a5d-114">Not supported.</span></span>|
|<span data-ttu-id="b6a5d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6a5d-115">Application</span></span>|<span data-ttu-id="b6a5d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a5d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6a5d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6a5d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="b6a5d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6a5d-118">Request headers</span></span>
|<span data-ttu-id="b6a5d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6a5d-119">Header</span></span>|<span data-ttu-id="b6a5d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b6a5d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6a5d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6a5d-121">Authorization</span></span>|<span data-ttu-id="b6a5d-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b6a5d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6a5d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b6a5d-123">Accept</span></span>|<span data-ttu-id="b6a5d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b6a5d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6a5d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6a5d-125">Request body</span></span>
<span data-ttu-id="b6a5d-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6a5d-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b6a5d-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b6a5d-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b6a5d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6a5d-128">Property</span></span>|<span data-ttu-id="b6a5d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b6a5d-129">Type</span></span>|<span data-ttu-id="b6a5d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b6a5d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6a5d-131">assignments</span><span class="sxs-lookup"><span data-stu-id="b6a5d-131">assignments</span></span>|<span data-ttu-id="b6a5d-132">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b6a5d-132">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b6a5d-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b6a5d-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b6a5d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6a5d-134">Response</span></span>
<span data-ttu-id="b6a5d-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b6a5d-135">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6a5d-136">Пример</span><span class="sxs-lookup"><span data-stu-id="b6a5d-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6a5d-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6a5d-137">Request</span></span>
<span data-ttu-id="b6a5d-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6a5d-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 277

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b6a5d-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6a5d-139">Response</span></span>
<span data-ttu-id="b6a5d-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b6a5d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



