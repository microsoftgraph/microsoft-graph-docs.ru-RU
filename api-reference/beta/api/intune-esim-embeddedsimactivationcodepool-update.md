---
title: Обновление embeddedSIMActivationCodePool
description: Обновление свойства объекта embeddedSIMActivationCodePool.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1894e0702f2d49cff86e9b7510c94eac5cbd0134
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404444"
---
# <a name="update-embeddedsimactivationcodepool"></a><span data-ttu-id="d565e-103">Обновление embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="d565e-103">Update embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="d565e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d565e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d565e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d565e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d565e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d565e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d565e-107">Обновление свойства объекта [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="d565e-107">Update the properties of a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d565e-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="d565e-108">Prerequisites</span></span>
<span data-ttu-id="d565e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d565e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d565e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d565e-111">Permission type</span></span>|<span data-ttu-id="d565e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d565e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d565e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d565e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d565e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d565e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d565e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d565e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d565e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d565e-116">Not supported.</span></span>|
|<span data-ttu-id="d565e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d565e-117">Application</span></span>|<span data-ttu-id="d565e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d565e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d565e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d565e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a><span data-ttu-id="d565e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d565e-120">Request headers</span></span>
|<span data-ttu-id="d565e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d565e-121">Header</span></span>|<span data-ttu-id="d565e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d565e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d565e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d565e-123">Authorization</span></span>|<span data-ttu-id="d565e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d565e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d565e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d565e-125">Accept</span></span>|<span data-ttu-id="d565e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d565e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d565e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d565e-127">Request body</span></span>
<span data-ttu-id="d565e-128">В тексте запроса укажите представление JSON для объекта [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="d565e-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

<span data-ttu-id="d565e-129">В следующей таблице показаны свойства, которые необходимы для создания [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span><span class="sxs-lookup"><span data-stu-id="d565e-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>

|<span data-ttu-id="d565e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d565e-130">Property</span></span>|<span data-ttu-id="d565e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d565e-131">Type</span></span>|<span data-ttu-id="d565e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d565e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d565e-133">id</span><span class="sxs-lookup"><span data-stu-id="d565e-133">id</span></span>|<span data-ttu-id="d565e-134">String</span><span class="sxs-lookup"><span data-stu-id="d565e-134">String</span></span>|<span data-ttu-id="d565e-135">Уникальный идентификатор для внедренных пула кода активации диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="d565e-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="d565e-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="d565e-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="d565e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d565e-137">displayName</span></span>|<span data-ttu-id="d565e-138">String</span><span class="sxs-lookup"><span data-stu-id="d565e-138">String</span></span>|<span data-ttu-id="d565e-139">Имя группы внедренных диспетчера установки активации кода определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="d565e-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="d565e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d565e-140">createdDateTime</span></span>|<span data-ttu-id="d565e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d565e-141">DateTimeOffset</span></span>|<span data-ttu-id="d565e-142">Время создания внедренных пула кода активации диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="d565e-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="d565e-143">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="d565e-143">Generated service side.</span></span>|
|<span data-ttu-id="d565e-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d565e-144">modifiedDateTime</span></span>|<span data-ttu-id="d565e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d565e-145">DateTimeOffset</span></span>|<span data-ttu-id="d565e-146">Время последнего изменения внедренного пула кода активации диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="d565e-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="d565e-147">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="d565e-147">Updated service side.</span></span>|
|<span data-ttu-id="d565e-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="d565e-148">activationCodes</span></span>|<span data-ttu-id="d565e-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="d565e-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="d565e-150">Коды активации, которые относятся к этот пул.</span><span class="sxs-lookup"><span data-stu-id="d565e-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="d565e-151">Это свойство навигации использовать для активации кодов Intune, но не может использоваться для чтения из Intune коды активации.</span><span class="sxs-lookup"><span data-stu-id="d565e-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="d565e-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="d565e-152">activationCodeCount</span></span>|<span data-ttu-id="d565e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d565e-153">Int32</span></span>|<span data-ttu-id="d565e-154">Общее число коды активации, которые относятся к этот пул.</span><span class="sxs-lookup"><span data-stu-id="d565e-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="d565e-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="d565e-155">Response</span></span>
<span data-ttu-id="d565e-156">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d565e-156">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d565e-157">Пример</span><span class="sxs-lookup"><span data-stu-id="d565e-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="d565e-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="d565e-158">Request</span></span>
<span data-ttu-id="d565e-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d565e-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
Content-type: application/json
Content-length: 460

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "displayName": "Display Name value",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```

### <a name="response"></a><span data-ttu-id="d565e-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="d565e-160">Response</span></span>
<span data-ttu-id="d565e-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d565e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 628

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "ec308741-8741-ec30-4187-30ec418730ec",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```




