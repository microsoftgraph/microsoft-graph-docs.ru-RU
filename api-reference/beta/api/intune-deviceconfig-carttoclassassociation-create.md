---
title: Создание cartToClassAssociation
description: Создание нового объекта cartToClassAssociation.
ms.openlocfilehash: 87e4a21a998e4226d429bfd92fca5560b9d716e3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081819"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="fc1eb-103">Создание cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="fc1eb-103">Create cartToClassAssociation</span></span>

> <span data-ttu-id="fc1eb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc1eb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc1eb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc1eb-107">Создание нового объекта [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="fc1eb-107">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fc1eb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fc1eb-108">Prerequisites</span></span>
<span data-ttu-id="fc1eb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc1eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc1eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc1eb-111">Permission type</span></span>|<span data-ttu-id="fc1eb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc1eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc1eb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc1eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc1eb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc1eb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fc1eb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc1eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc1eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-116">Not supported.</span></span>|
|<span data-ttu-id="fc1eb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc1eb-117">Application</span></span>|<span data-ttu-id="fc1eb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc1eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc1eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="fc1eb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc1eb-120">Request headers</span></span>
|<span data-ttu-id="fc1eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc1eb-121">Header</span></span>|<span data-ttu-id="fc1eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fc1eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc1eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc1eb-123">Authorization</span></span>|<span data-ttu-id="fc1eb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fc1eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc1eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fc1eb-125">Accept</span></span>|<span data-ttu-id="fc1eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc1eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc1eb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc1eb-127">Request body</span></span>
<span data-ttu-id="fc1eb-128">В тексте запроса укажите представление JSON для объекта cartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-128">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="fc1eb-129">В следующей таблице показаны свойства, которые необходимы для создания cartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-129">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="fc1eb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc1eb-130">Property</span></span>|<span data-ttu-id="fc1eb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fc1eb-131">Type</span></span>|<span data-ttu-id="fc1eb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fc1eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc1eb-133">id</span><span class="sxs-lookup"><span data-stu-id="fc1eb-133">id</span></span>|<span data-ttu-id="fc1eb-134">String</span><span class="sxs-lookup"><span data-stu-id="fc1eb-134">String</span></span>|<span data-ttu-id="fc1eb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-135">Key of the entity.</span></span>|
|<span data-ttu-id="fc1eb-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc1eb-136">createdDateTime</span></span>|<span data-ttu-id="fc1eb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc1eb-137">DateTimeOffset</span></span>|<span data-ttu-id="fc1eb-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="fc1eb-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc1eb-139">lastModifiedDateTime</span></span>|<span data-ttu-id="fc1eb-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc1eb-140">DateTimeOffset</span></span>|<span data-ttu-id="fc1eb-141">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="fc1eb-142">version</span><span class="sxs-lookup"><span data-stu-id="fc1eb-142">version</span></span>|<span data-ttu-id="fc1eb-143">Int32</span><span class="sxs-lookup"><span data-stu-id="fc1eb-143">Int32</span></span>|<span data-ttu-id="fc1eb-144">Версия CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="fc1eb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="fc1eb-145">displayName</span></span>|<span data-ttu-id="fc1eb-146">String</span><span class="sxs-lookup"><span data-stu-id="fc1eb-146">String</span></span>|<span data-ttu-id="fc1eb-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="fc1eb-148">описание</span><span class="sxs-lookup"><span data-stu-id="fc1eb-148">description</span></span>|<span data-ttu-id="fc1eb-149">String</span><span class="sxs-lookup"><span data-stu-id="fc1eb-149">String</span></span>|<span data-ttu-id="fc1eb-150">Admin, предоставляемые описание CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="fc1eb-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="fc1eb-151">deviceCartIds</span></span>|<span data-ttu-id="fc1eb-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc1eb-152">String collection</span></span>|<span data-ttu-id="fc1eb-153">Идентификаторы корзины устройства необходимо сопоставить с классы.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="fc1eb-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="fc1eb-154">classroomIds</span></span>|<span data-ttu-id="fc1eb-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc1eb-155">String collection</span></span>|<span data-ttu-id="fc1eb-156">Идентификаторы аудиторий необходимо сопоставить с устройства корзины.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="fc1eb-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc1eb-157">Response</span></span>
<span data-ttu-id="fc1eb-158">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-158">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc1eb-159">Пример</span><span class="sxs-lookup"><span data-stu-id="fc1eb-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="fc1eb-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc1eb-160">Request</span></span>
<span data-ttu-id="fc1eb-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc1eb-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
Content-type: application/json
Content-length: 335

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="fc1eb-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc1eb-162">Response</span></span>
<span data-ttu-id="fc1eb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="fc1eb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```





