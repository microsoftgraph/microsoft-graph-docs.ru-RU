---
title: Создание embeddedSIMActivationCodePool
description: Создание нового объекта embeddedSIMActivationCodePool.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a46245cb8f0a246363b5b1112298c360c3a4c24d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973701"
---
# <a name="create-embeddedsimactivationcodepool"></a><span data-ttu-id="e852b-103">Создание embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="e852b-103">Create embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="e852b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e852b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e852b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e852b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e852b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e852b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e852b-107">Создание нового объекта [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="e852b-107">Create a new [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e852b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e852b-108">Prerequisites</span></span>
<span data-ttu-id="e852b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e852b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e852b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e852b-111">Permission type</span></span>|<span data-ttu-id="e852b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e852b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e852b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e852b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e852b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e852b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e852b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e852b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e852b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e852b-116">Not supported.</span></span>|
|<span data-ttu-id="e852b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e852b-117">Application</span></span>|<span data-ttu-id="e852b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e852b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e852b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e852b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="e852b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e852b-120">Request headers</span></span>
|<span data-ttu-id="e852b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e852b-121">Header</span></span>|<span data-ttu-id="e852b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e852b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e852b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e852b-123">Authorization</span></span>|<span data-ttu-id="e852b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e852b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e852b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e852b-125">Accept</span></span>|<span data-ttu-id="e852b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e852b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e852b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e852b-127">Request body</span></span>
<span data-ttu-id="e852b-128">В тексте запроса укажите представление JSON для объекта embeddedSIMActivationCodePool.</span><span class="sxs-lookup"><span data-stu-id="e852b-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePool object.</span></span>

<span data-ttu-id="e852b-129">В следующей таблице показаны свойства, которые необходимы для создания embeddedSIMActivationCodePool.</span><span class="sxs-lookup"><span data-stu-id="e852b-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePool.</span></span>

|<span data-ttu-id="e852b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e852b-130">Property</span></span>|<span data-ttu-id="e852b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e852b-131">Type</span></span>|<span data-ttu-id="e852b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e852b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e852b-133">id</span><span class="sxs-lookup"><span data-stu-id="e852b-133">id</span></span>|<span data-ttu-id="e852b-134">String</span><span class="sxs-lookup"><span data-stu-id="e852b-134">String</span></span>|<span data-ttu-id="e852b-135">Уникальный идентификатор для внедренных пула кода активации диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="e852b-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="e852b-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="e852b-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="e852b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e852b-137">displayName</span></span>|<span data-ttu-id="e852b-138">String</span><span class="sxs-lookup"><span data-stu-id="e852b-138">String</span></span>|<span data-ttu-id="e852b-139">Имя группы внедренных диспетчера установки активации кода определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="e852b-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="e852b-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e852b-140">createdDateTime</span></span>|<span data-ttu-id="e852b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e852b-141">DateTimeOffset</span></span>|<span data-ttu-id="e852b-142">Время создания внедренных пула кода активации диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="e852b-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="e852b-143">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="e852b-143">Generated service side.</span></span>|
|<span data-ttu-id="e852b-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e852b-144">modifiedDateTime</span></span>|<span data-ttu-id="e852b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e852b-145">DateTimeOffset</span></span>|<span data-ttu-id="e852b-146">Время последнего изменения внедренного пула кода активации диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="e852b-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="e852b-147">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="e852b-147">Updated service side.</span></span>|
|<span data-ttu-id="e852b-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="e852b-148">activationCodes</span></span>|<span data-ttu-id="e852b-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e852b-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="e852b-150">Коды активации, которые относятся к этот пул.</span><span class="sxs-lookup"><span data-stu-id="e852b-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="e852b-151">Это свойство навигации использовать для активации кодов Intune, но не может использоваться для чтения из Intune коды активации.</span><span class="sxs-lookup"><span data-stu-id="e852b-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="e852b-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="e852b-152">activationCodeCount</span></span>|<span data-ttu-id="e852b-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e852b-153">Int32</span></span>|<span data-ttu-id="e852b-154">Общее число коды активации, которые относятся к этот пул.</span><span class="sxs-lookup"><span data-stu-id="e852b-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="e852b-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="e852b-155">Response</span></span>
<span data-ttu-id="e852b-156">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e852b-156">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e852b-157">Пример</span><span class="sxs-lookup"><span data-stu-id="e852b-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="e852b-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="e852b-158">Request</span></span>
<span data-ttu-id="e852b-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e852b-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
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

### <a name="response"></a><span data-ttu-id="e852b-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="e852b-160">Response</span></span>
<span data-ttu-id="e852b-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e852b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





