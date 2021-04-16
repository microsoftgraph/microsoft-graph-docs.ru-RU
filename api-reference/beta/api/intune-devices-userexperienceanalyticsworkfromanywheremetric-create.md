---
title: Создание userExperienceAnalyticsWorkFromAnywhereMetric
description: Создание нового объекта userExperienceAnalyticsWorkFromAnywhereMetric.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f33a06a7c9f9f256476319464a79fadcf680e709
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869004"
---
# <a name="create-userexperienceanalyticsworkfromanywheremetric"></a><span data-ttu-id="d655e-103">Создание userExperienceAnalyticsWorkFromAnywhereMetric</span><span class="sxs-lookup"><span data-stu-id="d655e-103">Create userExperienceAnalyticsWorkFromAnywhereMetric</span></span>

<span data-ttu-id="d655e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d655e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d655e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d655e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d655e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d655e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d655e-107">Создание нового [объекта userExperienceAnalyticsWorkFromAnywhereMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md)</span><span class="sxs-lookup"><span data-stu-id="d655e-107">Create a new [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d655e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d655e-108">Prerequisites</span></span>
<span data-ttu-id="d655e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d655e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d655e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d655e-111">Permission type</span></span>|<span data-ttu-id="d655e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d655e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d655e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d655e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d655e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d655e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d655e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d655e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d655e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d655e-116">Not supported.</span></span>|
|<span data-ttu-id="d655e-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d655e-117">Application</span></span>|<span data-ttu-id="d655e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d655e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d655e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d655e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics
```

## <a name="request-headers"></a><span data-ttu-id="d655e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d655e-120">Request headers</span></span>
|<span data-ttu-id="d655e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d655e-121">Header</span></span>|<span data-ttu-id="d655e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d655e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d655e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d655e-123">Authorization</span></span>|<span data-ttu-id="d655e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d655e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d655e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d655e-125">Accept</span></span>|<span data-ttu-id="d655e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d655e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d655e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d655e-127">Request body</span></span>
<span data-ttu-id="d655e-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsWorkFromAnywhereMetric.</span><span class="sxs-lookup"><span data-stu-id="d655e-128">In the request body, supply a JSON representation for the userExperienceAnalyticsWorkFromAnywhereMetric object.</span></span>

<span data-ttu-id="d655e-129">В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsWorkFromAnywhereMetric.</span><span class="sxs-lookup"><span data-stu-id="d655e-129">The following table shows the properties that are required when you create the userExperienceAnalyticsWorkFromAnywhereMetric.</span></span>

|<span data-ttu-id="d655e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d655e-130">Property</span></span>|<span data-ttu-id="d655e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d655e-131">Type</span></span>|<span data-ttu-id="d655e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d655e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d655e-133">id</span><span class="sxs-lookup"><span data-stu-id="d655e-133">id</span></span>|<span data-ttu-id="d655e-134">String</span><span class="sxs-lookup"><span data-stu-id="d655e-134">String</span></span>|<span data-ttu-id="d655e-135">Уникальный идентификатор аналитики пользовательских интерфейсов работает из любой метрики.</span><span class="sxs-lookup"><span data-stu-id="d655e-135">The unique identifier of the user experience analytics work from anywhere metric.</span></span>|



## <a name="response"></a><span data-ttu-id="d655e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d655e-136">Response</span></span>
<span data-ttu-id="d655e-137">В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d655e-137">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d655e-138">Пример</span><span class="sxs-lookup"><span data-stu-id="d655e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d655e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d655e-139">Request</span></span>
<span data-ttu-id="d655e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d655e-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics
Content-type: application/json
Content-length: 87

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereMetric"
}
```

### <a name="response"></a><span data-ttu-id="d655e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d655e-141">Response</span></span>
<span data-ttu-id="d655e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d655e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 136

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereMetric",
  "id": "7e6fda96-da96-7e6f-96da-6f7e96da6f7e"
}
```




