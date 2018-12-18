---
title: Обновление cartToClassAssociation
description: Обновление свойства объекта cartToClassAssociation.
author: tfitzmac
ms.openlocfilehash: 43b272a5fa2871daebbf7cfeea890ba0b9e204e8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343018"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="5d830-103">Обновление cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="5d830-103">Update cartToClassAssociation</span></span>

> <span data-ttu-id="5d830-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5d830-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d830-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d830-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d830-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5d830-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d830-107">Обновление свойства объекта [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="5d830-107">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5d830-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5d830-108">Prerequisites</span></span>
<span data-ttu-id="5d830-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d830-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d830-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d830-111">Permission type</span></span>|<span data-ttu-id="5d830-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d830-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d830-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d830-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d830-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d830-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5d830-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d830-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d830-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d830-116">Not supported.</span></span>|
|<span data-ttu-id="5d830-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d830-117">Application</span></span>|<span data-ttu-id="5d830-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d830-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d830-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d830-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="5d830-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d830-120">Request headers</span></span>
|<span data-ttu-id="5d830-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d830-121">Header</span></span>|<span data-ttu-id="5d830-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5d830-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d830-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d830-123">Authorization</span></span>|<span data-ttu-id="5d830-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5d830-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d830-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5d830-125">Accept</span></span>|<span data-ttu-id="5d830-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d830-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d830-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d830-127">Request body</span></span>
<span data-ttu-id="5d830-128">В тексте запроса укажите представление JSON для объекта [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="5d830-128">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="5d830-129">В следующей таблице показаны свойства, которые необходимы для создания [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span><span class="sxs-lookup"><span data-stu-id="5d830-129">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="5d830-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d830-130">Property</span></span>|<span data-ttu-id="5d830-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5d830-131">Type</span></span>|<span data-ttu-id="5d830-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5d830-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d830-133">id</span><span class="sxs-lookup"><span data-stu-id="5d830-133">id</span></span>|<span data-ttu-id="5d830-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5d830-134">String</span></span>|<span data-ttu-id="5d830-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5d830-135">Key of the entity.</span></span>|
|<span data-ttu-id="5d830-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5d830-136">createdDateTime</span></span>|<span data-ttu-id="5d830-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d830-137">DateTimeOffset</span></span>|<span data-ttu-id="5d830-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5d830-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="5d830-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d830-139">lastModifiedDateTime</span></span>|<span data-ttu-id="5d830-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d830-140">DateTimeOffset</span></span>|<span data-ttu-id="5d830-141">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5d830-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="5d830-142">version</span><span class="sxs-lookup"><span data-stu-id="5d830-142">version</span></span>|<span data-ttu-id="5d830-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5d830-143">Int32</span></span>|<span data-ttu-id="5d830-144">Версия CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="5d830-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="5d830-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5d830-145">displayName</span></span>|<span data-ttu-id="5d830-146">Строка</span><span class="sxs-lookup"><span data-stu-id="5d830-146">String</span></span>|<span data-ttu-id="5d830-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5d830-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="5d830-148">описание</span><span class="sxs-lookup"><span data-stu-id="5d830-148">description</span></span>|<span data-ttu-id="5d830-149">Строка</span><span class="sxs-lookup"><span data-stu-id="5d830-149">String</span></span>|<span data-ttu-id="5d830-150">Admin, предоставляемые описание CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="5d830-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="5d830-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="5d830-151">deviceCartIds</span></span>|<span data-ttu-id="5d830-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5d830-152">String collection</span></span>|<span data-ttu-id="5d830-153">Идентификаторы корзины устройства необходимо сопоставить с классы.</span><span class="sxs-lookup"><span data-stu-id="5d830-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="5d830-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="5d830-154">classroomIds</span></span>|<span data-ttu-id="5d830-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5d830-155">String collection</span></span>|<span data-ttu-id="5d830-156">Идентификаторы аудиторий необходимо сопоставить с устройства корзины.</span><span class="sxs-lookup"><span data-stu-id="5d830-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="5d830-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="5d830-157">Response</span></span>
<span data-ttu-id="5d830-158">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5d830-158">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d830-159">Пример</span><span class="sxs-lookup"><span data-stu-id="5d830-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="5d830-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d830-160">Request</span></span>
<span data-ttu-id="5d830-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d830-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
Content-type: application/json
Content-length: 274

{
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

### <a name="response"></a><span data-ttu-id="5d830-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="5d830-162">Response</span></span>
<span data-ttu-id="5d830-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5d830-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





