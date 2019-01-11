---
title: Создание embeddedSIMActivationCodePoolAssignment
description: Создание нового объекта embeddedSIMActivationCodePoolAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e020dafec47fe1a669251825ba0dff75f41f382c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865935"
---
# <a name="create-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="85f2b-103">Создание embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="85f2b-103">Create embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="85f2b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="85f2b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85f2b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85f2b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85f2b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="85f2b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85f2b-107">Создание нового объекта [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="85f2b-107">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85f2b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="85f2b-108">Prerequisites</span></span>
<span data-ttu-id="85f2b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85f2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85f2b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85f2b-111">Permission type</span></span>|<span data-ttu-id="85f2b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85f2b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85f2b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85f2b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85f2b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85f2b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85f2b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85f2b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85f2b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85f2b-116">Not supported.</span></span>|
|<span data-ttu-id="85f2b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85f2b-117">Application</span></span>|<span data-ttu-id="85f2b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85f2b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85f2b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85f2b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="85f2b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85f2b-120">Request headers</span></span>
|<span data-ttu-id="85f2b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85f2b-121">Header</span></span>|<span data-ttu-id="85f2b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="85f2b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85f2b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85f2b-123">Authorization</span></span>|<span data-ttu-id="85f2b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="85f2b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85f2b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="85f2b-125">Accept</span></span>|<span data-ttu-id="85f2b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85f2b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85f2b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85f2b-127">Request body</span></span>
<span data-ttu-id="85f2b-128">В тексте запроса укажите представление JSON для объекта embeddedSIMActivationCodePoolAssignment.</span><span class="sxs-lookup"><span data-stu-id="85f2b-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePoolAssignment object.</span></span>

<span data-ttu-id="85f2b-129">В следующей таблице показаны свойства, которые необходимы для создания embeddedSIMActivationCodePoolAssignment.</span><span class="sxs-lookup"><span data-stu-id="85f2b-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePoolAssignment.</span></span>

|<span data-ttu-id="85f2b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="85f2b-130">Property</span></span>|<span data-ttu-id="85f2b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="85f2b-131">Type</span></span>|<span data-ttu-id="85f2b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="85f2b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85f2b-133">id</span><span class="sxs-lookup"><span data-stu-id="85f2b-133">id</span></span>|<span data-ttu-id="85f2b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="85f2b-134">String</span></span>|<span data-ttu-id="85f2b-135">Уникальный идентификатор для диспетчера установки активации кода пул назначений.</span><span class="sxs-lookup"><span data-stu-id="85f2b-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="85f2b-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="85f2b-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="85f2b-137">target</span><span class="sxs-lookup"><span data-stu-id="85f2b-137">target</span></span>|[<span data-ttu-id="85f2b-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="85f2b-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="85f2b-139">Тип группы, входят в целевую внедренных пула кода активации диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="85f2b-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="85f2b-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="85f2b-140">Response</span></span>
<span data-ttu-id="85f2b-141">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="85f2b-141">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85f2b-142">Пример</span><span class="sxs-lookup"><span data-stu-id="85f2b-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="85f2b-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="85f2b-143">Request</span></span>
<span data-ttu-id="85f2b-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85f2b-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="85f2b-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="85f2b-145">Response</span></span>
<span data-ttu-id="85f2b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="85f2b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





