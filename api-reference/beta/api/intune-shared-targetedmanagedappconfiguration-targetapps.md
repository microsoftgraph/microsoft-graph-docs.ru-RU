---
title: Действие targetApps
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5638b08442fe8b08e38ddb5372200cbbbb2c609
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536933"
---
# <a name="targetapps-action"></a><span data-ttu-id="44597-103">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="44597-103">targetApps action</span></span>

> <span data-ttu-id="44597-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44597-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44597-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44597-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44597-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="44597-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44597-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="44597-107">Prerequisites</span></span>
<span data-ttu-id="44597-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44597-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44597-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44597-110">Permission type</span></span>|<span data-ttu-id="44597-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44597-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44597-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44597-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="44597-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="44597-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="44597-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44597-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="44597-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44597-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44597-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44597-116">Not supported.</span></span>|
|<span data-ttu-id="44597-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="44597-117">Application</span></span>||
| <span data-ttu-id="44597-118">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="44597-118">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="44597-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44597-119">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44597-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44597-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="44597-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44597-121">Request headers</span></span>
|<span data-ttu-id="44597-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44597-122">Header</span></span>|<span data-ttu-id="44597-123">Значение</span><span class="sxs-lookup"><span data-stu-id="44597-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44597-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44597-124">Authorization</span></span>|<span data-ttu-id="44597-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44597-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44597-126">Accept</span><span class="sxs-lookup"><span data-stu-id="44597-126">Accept</span></span>|<span data-ttu-id="44597-127">application/json</span><span class="sxs-lookup"><span data-stu-id="44597-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44597-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44597-128">Request body</span></span>
<span data-ttu-id="44597-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44597-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="44597-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="44597-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="44597-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="44597-131">Property</span></span>|<span data-ttu-id="44597-132">Тип</span><span class="sxs-lookup"><span data-stu-id="44597-132">Type</span></span>|<span data-ttu-id="44597-133">Описание</span><span class="sxs-lookup"><span data-stu-id="44597-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44597-134">apps</span><span class="sxs-lookup"><span data-stu-id="44597-134">apps</span></span>|<span data-ttu-id="44597-135">Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44597-135">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="44597-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="44597-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="44597-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="44597-137">Response</span></span>
<span data-ttu-id="44597-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="44597-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="44597-139">Пример</span><span class="sxs-lookup"><span data-stu-id="44597-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="44597-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="44597-140">Request</span></span>
<span data-ttu-id="44597-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44597-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="44597-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="44597-142">Response</span></span>
<span data-ttu-id="44597-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44597-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






