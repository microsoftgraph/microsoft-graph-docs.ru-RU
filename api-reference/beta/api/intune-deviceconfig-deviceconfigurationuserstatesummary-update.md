---
title: Обновление deviceConfigurationUserStateSummary
description: Обновление свойства объекта deviceConfigurationUserStateSummary.
author: tfitzmac
ms.openlocfilehash: a11c4447fee84116b68416ba78f610e8067a6104
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301570"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="d59e8-103">Обновление deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="d59e8-103">Update deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="d59e8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d59e8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d59e8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d59e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d59e8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d59e8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d59e8-107">Обновление свойства объекта [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d59e8-107">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d59e8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d59e8-108">Prerequisites</span></span>
<span data-ttu-id="d59e8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d59e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d59e8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d59e8-111">Permission type</span></span>|<span data-ttu-id="d59e8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d59e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d59e8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d59e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d59e8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d59e8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d59e8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d59e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d59e8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d59e8-116">Not supported.</span></span>|
|<span data-ttu-id="d59e8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d59e8-117">Application</span></span>|<span data-ttu-id="d59e8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d59e8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d59e8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d59e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="d59e8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d59e8-120">Request headers</span></span>
|<span data-ttu-id="d59e8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d59e8-121">Header</span></span>|<span data-ttu-id="d59e8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d59e8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d59e8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d59e8-123">Authorization</span></span>|<span data-ttu-id="d59e8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d59e8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d59e8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d59e8-125">Accept</span></span>|<span data-ttu-id="d59e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d59e8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d59e8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d59e8-127">Request body</span></span>
<span data-ttu-id="d59e8-128">В тексте запроса укажите представление JSON для объекта [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d59e8-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="d59e8-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d59e8-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="d59e8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d59e8-130">Property</span></span>|<span data-ttu-id="d59e8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d59e8-131">Type</span></span>|<span data-ttu-id="d59e8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d59e8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d59e8-133">id</span><span class="sxs-lookup"><span data-stu-id="d59e8-133">id</span></span>|<span data-ttu-id="d59e8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d59e8-134">String</span></span>|<span data-ttu-id="d59e8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d59e8-135">Key of the entity.</span></span>|
|<span data-ttu-id="d59e8-136">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="d59e8-136">unknownUserCount</span></span>|<span data-ttu-id="d59e8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d59e8-137">Int32</span></span>|<span data-ttu-id="d59e8-138">Число неизвестным пользователям</span><span class="sxs-lookup"><span data-stu-id="d59e8-138">Number of unknown users</span></span>|
|<span data-ttu-id="d59e8-139">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="d59e8-139">notApplicableUserCount</span></span>|<span data-ttu-id="d59e8-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d59e8-140">Int32</span></span>|<span data-ttu-id="d59e8-141">Число пользователей не применим</span><span class="sxs-lookup"><span data-stu-id="d59e8-141">Number of not applicable users</span></span>|
|<span data-ttu-id="d59e8-142">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="d59e8-142">compliantUserCount</span></span>|<span data-ttu-id="d59e8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d59e8-143">Int32</span></span>|<span data-ttu-id="d59e8-144">Количество требованиям пользователей</span><span class="sxs-lookup"><span data-stu-id="d59e8-144">Number of compliant users</span></span>|
|<span data-ttu-id="d59e8-145">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="d59e8-145">remediatedUserCount</span></span>|<span data-ttu-id="d59e8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d59e8-146">Int32</span></span>|<span data-ttu-id="d59e8-147">Количество проверка пользователей</span><span class="sxs-lookup"><span data-stu-id="d59e8-147">Number of remediated users</span></span>|
|<span data-ttu-id="d59e8-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="d59e8-148">nonCompliantUserCount</span></span>|<span data-ttu-id="d59e8-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d59e8-149">Int32</span></span>|<span data-ttu-id="d59e8-150">Количество несовместимой пользователей</span><span class="sxs-lookup"><span data-stu-id="d59e8-150">Number of NonCompliant users</span></span>|
|<span data-ttu-id="d59e8-151">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="d59e8-151">errorUserCount</span></span>|<span data-ttu-id="d59e8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d59e8-152">Int32</span></span>|<span data-ttu-id="d59e8-153">Число пользователей об ошибках</span><span class="sxs-lookup"><span data-stu-id="d59e8-153">Number of error users</span></span>|
|<span data-ttu-id="d59e8-154">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="d59e8-154">conflictUserCount</span></span>|<span data-ttu-id="d59e8-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d59e8-155">Int32</span></span>|<span data-ttu-id="d59e8-156">Число пользователей конфликта</span><span class="sxs-lookup"><span data-stu-id="d59e8-156">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="d59e8-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="d59e8-157">Response</span></span>
<span data-ttu-id="d59e8-158">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d59e8-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d59e8-159">Пример</span><span class="sxs-lookup"><span data-stu-id="d59e8-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="d59e8-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="d59e8-160">Request</span></span>
<span data-ttu-id="d59e8-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d59e8-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d59e8-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="d59e8-162">Response</span></span>
<span data-ttu-id="d59e8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d59e8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





