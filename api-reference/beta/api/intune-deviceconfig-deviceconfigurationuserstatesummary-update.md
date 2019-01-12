---
title: Обновление deviceConfigurationUserStateSummary
description: Обновление свойства объекта deviceConfigurationUserStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7bce2ebe487805526ab51199c13dc5d65215175d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933171"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="7b70a-103">Обновление deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="7b70a-103">Update deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="7b70a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b70a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b70a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b70a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b70a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7b70a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b70a-107">Обновление свойства объекта [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="7b70a-107">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b70a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7b70a-108">Prerequisites</span></span>
<span data-ttu-id="7b70a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b70a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b70a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b70a-111">Permission type</span></span>|<span data-ttu-id="7b70a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b70a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b70a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b70a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b70a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b70a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b70a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b70a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b70a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b70a-116">Not supported.</span></span>|
|<span data-ttu-id="7b70a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b70a-117">Application</span></span>|<span data-ttu-id="7b70a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b70a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b70a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b70a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="7b70a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b70a-120">Request headers</span></span>
|<span data-ttu-id="7b70a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b70a-121">Header</span></span>|<span data-ttu-id="7b70a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7b70a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b70a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b70a-123">Authorization</span></span>|<span data-ttu-id="7b70a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7b70a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b70a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7b70a-125">Accept</span></span>|<span data-ttu-id="7b70a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b70a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b70a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b70a-127">Request body</span></span>
<span data-ttu-id="7b70a-128">В тексте запроса укажите представление JSON для объекта [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="7b70a-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="7b70a-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7b70a-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="7b70a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b70a-130">Property</span></span>|<span data-ttu-id="7b70a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7b70a-131">Type</span></span>|<span data-ttu-id="7b70a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7b70a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b70a-133">id</span><span class="sxs-lookup"><span data-stu-id="7b70a-133">id</span></span>|<span data-ttu-id="7b70a-134">String</span><span class="sxs-lookup"><span data-stu-id="7b70a-134">String</span></span>|<span data-ttu-id="7b70a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7b70a-135">Key of the entity.</span></span>|
|<span data-ttu-id="7b70a-136">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="7b70a-136">unknownUserCount</span></span>|<span data-ttu-id="7b70a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7b70a-137">Int32</span></span>|<span data-ttu-id="7b70a-138">Число неизвестным пользователям</span><span class="sxs-lookup"><span data-stu-id="7b70a-138">Number of unknown users</span></span>|
|<span data-ttu-id="7b70a-139">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="7b70a-139">notApplicableUserCount</span></span>|<span data-ttu-id="7b70a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7b70a-140">Int32</span></span>|<span data-ttu-id="7b70a-141">Число пользователей не применим</span><span class="sxs-lookup"><span data-stu-id="7b70a-141">Number of not applicable users</span></span>|
|<span data-ttu-id="7b70a-142">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="7b70a-142">compliantUserCount</span></span>|<span data-ttu-id="7b70a-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7b70a-143">Int32</span></span>|<span data-ttu-id="7b70a-144">Количество требованиям пользователей</span><span class="sxs-lookup"><span data-stu-id="7b70a-144">Number of compliant users</span></span>|
|<span data-ttu-id="7b70a-145">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="7b70a-145">remediatedUserCount</span></span>|<span data-ttu-id="7b70a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="7b70a-146">Int32</span></span>|<span data-ttu-id="7b70a-147">Количество проверка пользователей</span><span class="sxs-lookup"><span data-stu-id="7b70a-147">Number of remediated users</span></span>|
|<span data-ttu-id="7b70a-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="7b70a-148">nonCompliantUserCount</span></span>|<span data-ttu-id="7b70a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="7b70a-149">Int32</span></span>|<span data-ttu-id="7b70a-150">Количество несовместимой пользователей</span><span class="sxs-lookup"><span data-stu-id="7b70a-150">Number of NonCompliant users</span></span>|
|<span data-ttu-id="7b70a-151">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="7b70a-151">errorUserCount</span></span>|<span data-ttu-id="7b70a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7b70a-152">Int32</span></span>|<span data-ttu-id="7b70a-153">Число пользователей об ошибках</span><span class="sxs-lookup"><span data-stu-id="7b70a-153">Number of error users</span></span>|
|<span data-ttu-id="7b70a-154">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="7b70a-154">conflictUserCount</span></span>|<span data-ttu-id="7b70a-155">Int32</span><span class="sxs-lookup"><span data-stu-id="7b70a-155">Int32</span></span>|<span data-ttu-id="7b70a-156">Число пользователей конфликта</span><span class="sxs-lookup"><span data-stu-id="7b70a-156">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="7b70a-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b70a-157">Response</span></span>
<span data-ttu-id="7b70a-158">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7b70a-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b70a-159">Пример</span><span class="sxs-lookup"><span data-stu-id="7b70a-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b70a-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b70a-160">Request</span></span>
<span data-ttu-id="7b70a-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b70a-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
Content-type: application/json
Content-length: 201

{
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```

### <a name="response"></a><span data-ttu-id="7b70a-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b70a-162">Response</span></span>
<span data-ttu-id="7b70a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7b70a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "e8957887-7887-e895-8778-95e8877895e8",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```





