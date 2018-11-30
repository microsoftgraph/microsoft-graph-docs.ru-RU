---
title: Обновление embeddedSIMActivationCodePool
description: Обновление свойства объекта embeddedSIMActivationCodePool.
ms.openlocfilehash: 50fc624840a19886e615f4acfe8b540c0fcf5ba0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078445"
---
# <a name="update-embeddedsimactivationcodepool"></a><span data-ttu-id="87dda-103">Обновление embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="87dda-103">Update embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="87dda-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="87dda-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87dda-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87dda-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87dda-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="87dda-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87dda-107">Обновление свойства объекта [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="87dda-107">Update the properties of a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87dda-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="87dda-108">Prerequisites</span></span>
<span data-ttu-id="87dda-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87dda-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87dda-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87dda-111">Permission type</span></span>|<span data-ttu-id="87dda-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87dda-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87dda-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87dda-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87dda-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87dda-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="87dda-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87dda-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87dda-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87dda-116">Not supported.</span></span>|
|<span data-ttu-id="87dda-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87dda-117">Application</span></span>|<span data-ttu-id="87dda-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87dda-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87dda-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87dda-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a><span data-ttu-id="87dda-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87dda-120">Request headers</span></span>
|<span data-ttu-id="87dda-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87dda-121">Header</span></span>|<span data-ttu-id="87dda-122">Значение</span><span class="sxs-lookup"><span data-stu-id="87dda-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87dda-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87dda-123">Authorization</span></span>|<span data-ttu-id="87dda-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="87dda-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87dda-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87dda-125">Accept</span></span>|<span data-ttu-id="87dda-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87dda-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87dda-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87dda-127">Request body</span></span>
<span data-ttu-id="87dda-128">В тексте запроса укажите представление JSON для объекта [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="87dda-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

<span data-ttu-id="87dda-129">В следующей таблице показаны свойства, которые необходимы для создания [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span><span class="sxs-lookup"><span data-stu-id="87dda-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>

|<span data-ttu-id="87dda-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="87dda-130">Property</span></span>|<span data-ttu-id="87dda-131">Тип</span><span class="sxs-lookup"><span data-stu-id="87dda-131">Type</span></span>|<span data-ttu-id="87dda-132">Описание</span><span class="sxs-lookup"><span data-stu-id="87dda-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87dda-133">id</span><span class="sxs-lookup"><span data-stu-id="87dda-133">id</span></span>|<span data-ttu-id="87dda-134">String</span><span class="sxs-lookup"><span data-stu-id="87dda-134">String</span></span>|<span data-ttu-id="87dda-135">Уникальный идентификатор для внедренных пула кода активации диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="87dda-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="87dda-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="87dda-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="87dda-137">displayName</span><span class="sxs-lookup"><span data-stu-id="87dda-137">displayName</span></span>|<span data-ttu-id="87dda-138">String</span><span class="sxs-lookup"><span data-stu-id="87dda-138">String</span></span>|<span data-ttu-id="87dda-139">Имя группы внедренных диспетчера установки активации кода определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="87dda-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="87dda-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87dda-140">createdDateTime</span></span>|<span data-ttu-id="87dda-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87dda-141">DateTimeOffset</span></span>|<span data-ttu-id="87dda-142">Время создания внедренных пула кода активации диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="87dda-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="87dda-143">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="87dda-143">Generated service side.</span></span>|
|<span data-ttu-id="87dda-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87dda-144">modifiedDateTime</span></span>|<span data-ttu-id="87dda-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87dda-145">DateTimeOffset</span></span>|<span data-ttu-id="87dda-146">Время последнего изменения внедренного пула кода активации диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="87dda-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="87dda-147">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="87dda-147">Updated service side.</span></span>|
|<span data-ttu-id="87dda-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="87dda-148">activationCodes</span></span>|<span data-ttu-id="87dda-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="87dda-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="87dda-150">Коды активации, которые относятся к этот пул.</span><span class="sxs-lookup"><span data-stu-id="87dda-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="87dda-151">Это свойство навигации использовать для активации кодов Intune, но не может использоваться для чтения из Intune коды активации.</span><span class="sxs-lookup"><span data-stu-id="87dda-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="87dda-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="87dda-152">activationCodeCount</span></span>|<span data-ttu-id="87dda-153">Int32</span><span class="sxs-lookup"><span data-stu-id="87dda-153">Int32</span></span>|<span data-ttu-id="87dda-154">Общее число коды активации, которые относятся к этот пул.</span><span class="sxs-lookup"><span data-stu-id="87dda-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="87dda-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="87dda-155">Response</span></span>
<span data-ttu-id="87dda-156">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="87dda-156">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87dda-157">Пример</span><span class="sxs-lookup"><span data-stu-id="87dda-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="87dda-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="87dda-158">Request</span></span>
<span data-ttu-id="87dda-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87dda-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
Content-type: application/json
Content-length: 392

{
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

### <a name="response"></a><span data-ttu-id="87dda-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="87dda-160">Response</span></span>
<span data-ttu-id="87dda-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="87dda-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





