---
title: Обновление embeddedSIMActivationCodePoolAssignment
description: Обновление свойства объекта embeddedSIMActivationCodePoolAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 87d2b3470107b1c517f29af4704b8038d85a7f54
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420796"
---
# <a name="update-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="008c6-103">Обновление embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="008c6-103">Update embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="008c6-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="008c6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="008c6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="008c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="008c6-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="008c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="008c6-107">Обновление свойства объекта [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="008c6-107">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="008c6-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="008c6-108">Prerequisites</span></span>
<span data-ttu-id="008c6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="008c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="008c6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="008c6-111">Permission type</span></span>|<span data-ttu-id="008c6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="008c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="008c6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="008c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="008c6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="008c6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="008c6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="008c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="008c6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="008c6-116">Not supported.</span></span>|
|<span data-ttu-id="008c6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="008c6-117">Application</span></span>|<span data-ttu-id="008c6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="008c6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="008c6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="008c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="008c6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="008c6-120">Request headers</span></span>
|<span data-ttu-id="008c6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="008c6-121">Header</span></span>|<span data-ttu-id="008c6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="008c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="008c6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="008c6-123">Authorization</span></span>|<span data-ttu-id="008c6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="008c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="008c6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="008c6-125">Accept</span></span>|<span data-ttu-id="008c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="008c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="008c6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="008c6-127">Request body</span></span>
<span data-ttu-id="008c6-128">В тексте запроса укажите представление JSON для объекта [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="008c6-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

<span data-ttu-id="008c6-129">В следующей таблице показаны свойства, которые необходимы для создания [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span><span class="sxs-lookup"><span data-stu-id="008c6-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

|<span data-ttu-id="008c6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="008c6-130">Property</span></span>|<span data-ttu-id="008c6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="008c6-131">Type</span></span>|<span data-ttu-id="008c6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="008c6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="008c6-133">id</span><span class="sxs-lookup"><span data-stu-id="008c6-133">id</span></span>|<span data-ttu-id="008c6-134">String</span><span class="sxs-lookup"><span data-stu-id="008c6-134">String</span></span>|<span data-ttu-id="008c6-135">Уникальный идентификатор для диспетчера установки активации кода пул назначений.</span><span class="sxs-lookup"><span data-stu-id="008c6-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="008c6-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="008c6-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="008c6-137">target</span><span class="sxs-lookup"><span data-stu-id="008c6-137">target</span></span>|[<span data-ttu-id="008c6-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="008c6-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="008c6-139">Тип группы, входят в целевую внедренных пула кода активации диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="008c6-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="008c6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="008c6-140">Response</span></span>
<span data-ttu-id="008c6-141">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="008c6-141">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="008c6-142">Пример</span><span class="sxs-lookup"><span data-stu-id="008c6-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="008c6-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="008c6-143">Request</span></span>
<span data-ttu-id="008c6-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="008c6-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="008c6-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="008c6-145">Response</span></span>
<span data-ttu-id="008c6-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="008c6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




