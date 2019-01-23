---
title: Действие assign
description: Замените все целевые группы для политики.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 37143c09382ae08b600aeacd6af02ebb44c86bf1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409260"
---
# <a name="assign-action"></a><span data-ttu-id="c7ebe-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="c7ebe-103">assign action</span></span>

> <span data-ttu-id="c7ebe-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c7ebe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7ebe-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7ebe-107">Замените все целевые группы для политики.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-107">Replace all targeted groups for a policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7ebe-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="c7ebe-108">Prerequisites</span></span>
<span data-ttu-id="c7ebe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7ebe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7ebe-111">Permission type</span></span>|<span data-ttu-id="c7ebe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7ebe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7ebe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7ebe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7ebe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7ebe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7ebe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7ebe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7ebe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-116">Not supported.</span></span>|
|<span data-ttu-id="c7ebe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7ebe-117">Application</span></span>|<span data-ttu-id="c7ebe-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7ebe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7ebe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="c7ebe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7ebe-120">Request headers</span></span>
|<span data-ttu-id="c7ebe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7ebe-121">Header</span></span>|<span data-ttu-id="c7ebe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7ebe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7ebe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7ebe-123">Authorization</span></span>|<span data-ttu-id="c7ebe-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c7ebe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7ebe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7ebe-125">Accept</span></span>|<span data-ttu-id="c7ebe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7ebe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7ebe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7ebe-127">Request body</span></span>
<span data-ttu-id="c7ebe-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c7ebe-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c7ebe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7ebe-130">Property</span></span>|<span data-ttu-id="c7ebe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c7ebe-131">Type</span></span>|<span data-ttu-id="c7ebe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c7ebe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7ebe-133">officeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="c7ebe-133">officeConfigurationAssignments</span></span>|<span data-ttu-id="c7ebe-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c7ebe-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c7ebe-135">Список назначений настройки office</span><span class="sxs-lookup"><span data-stu-id="c7ebe-135">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="c7ebe-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7ebe-136">Response</span></span>
<span data-ttu-id="c7ebe-137">Если успешно завершена, это действие возвращает `200 OK` код ответа и семейства [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-137">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7ebe-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c7ebe-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7ebe-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7ebe-139">Request</span></span>
<span data-ttu-id="c7ebe-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign

Content-type: application/json
Content-length: 299

{
  "officeConfigurationAssignments": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c7ebe-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7ebe-141">Response</span></span>
<span data-ttu-id="c7ebe-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```



