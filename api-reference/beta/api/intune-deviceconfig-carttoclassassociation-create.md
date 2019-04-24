---
title: Создание КарттоклассассоЦиатион
description: Создание нового объекта КарттоклассассоЦиатион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c683b2ae19caa55c62f0af834fbb8b74d5fb904c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32471583"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="02346-103">Создание КарттоклассассоЦиатион</span><span class="sxs-lookup"><span data-stu-id="02346-103">Create cartToClassAssociation</span></span>

> <span data-ttu-id="02346-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02346-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02346-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02346-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02346-106">Создание нового объекта [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="02346-106">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02346-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="02346-107">Prerequisites</span></span>
<span data-ttu-id="02346-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02346-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02346-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02346-110">Permission type</span></span>|<span data-ttu-id="02346-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="02346-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02346-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02346-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02346-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02346-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02346-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02346-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02346-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02346-115">Not supported.</span></span>|
|<span data-ttu-id="02346-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02346-116">Application</span></span>|<span data-ttu-id="02346-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02346-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02346-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02346-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="02346-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02346-119">Request headers</span></span>
|<span data-ttu-id="02346-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02346-120">Header</span></span>|<span data-ttu-id="02346-121">Значение</span><span class="sxs-lookup"><span data-stu-id="02346-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02346-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02346-122">Authorization</span></span>|<span data-ttu-id="02346-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02346-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02346-124">Accept</span><span class="sxs-lookup"><span data-stu-id="02346-124">Accept</span></span>|<span data-ttu-id="02346-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02346-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02346-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02346-126">Request body</span></span>
<span data-ttu-id="02346-127">В тексте запроса добавьте представление объекта КарттоклассассоЦиатион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02346-127">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="02346-128">В следующей таблице приведены свойства, необходимые при создании КарттоклассассоЦиатион.</span><span class="sxs-lookup"><span data-stu-id="02346-128">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="02346-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="02346-129">Property</span></span>|<span data-ttu-id="02346-130">Тип</span><span class="sxs-lookup"><span data-stu-id="02346-130">Type</span></span>|<span data-ttu-id="02346-131">Описание</span><span class="sxs-lookup"><span data-stu-id="02346-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02346-132">id</span><span class="sxs-lookup"><span data-stu-id="02346-132">id</span></span>|<span data-ttu-id="02346-133">Строка</span><span class="sxs-lookup"><span data-stu-id="02346-133">String</span></span>|<span data-ttu-id="02346-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="02346-134">Key of the entity.</span></span>|
|<span data-ttu-id="02346-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02346-135">createdDateTime</span></span>|<span data-ttu-id="02346-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02346-136">DateTimeOffset</span></span>|<span data-ttu-id="02346-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="02346-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="02346-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02346-138">lastModifiedDateTime</span></span>|<span data-ttu-id="02346-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02346-139">DateTimeOffset</span></span>|<span data-ttu-id="02346-140">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="02346-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="02346-141">version</span><span class="sxs-lookup"><span data-stu-id="02346-141">version</span></span>|<span data-ttu-id="02346-142">Int32</span><span class="sxs-lookup"><span data-stu-id="02346-142">Int32</span></span>|<span data-ttu-id="02346-143">Версия КарттоклассассоЦиатион.</span><span class="sxs-lookup"><span data-stu-id="02346-143">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="02346-144">displayName</span><span class="sxs-lookup"><span data-stu-id="02346-144">displayName</span></span>|<span data-ttu-id="02346-145">String</span><span class="sxs-lookup"><span data-stu-id="02346-145">String</span></span>|<span data-ttu-id="02346-146">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="02346-146">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="02346-147">description</span><span class="sxs-lookup"><span data-stu-id="02346-147">description</span></span>|<span data-ttu-id="02346-148">String</span><span class="sxs-lookup"><span data-stu-id="02346-148">String</span></span>|<span data-ttu-id="02346-149">Администратор предоставил описание КарттоклассассоЦиатион.</span><span class="sxs-lookup"><span data-stu-id="02346-149">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="02346-150">Девицекартидс</span><span class="sxs-lookup"><span data-stu-id="02346-150">deviceCartIds</span></span>|<span data-ttu-id="02346-151">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="02346-151">String collection</span></span>|<span data-ttu-id="02346-152">Идентификаторы корзин устройств, которые необходимо связать с классами.</span><span class="sxs-lookup"><span data-stu-id="02346-152">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="02346-153">Классрумидс</span><span class="sxs-lookup"><span data-stu-id="02346-153">classroomIds</span></span>|<span data-ttu-id="02346-154">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="02346-154">String collection</span></span>|<span data-ttu-id="02346-155">Идентификаторы аудиторий, которые необходимо связать с тележками устройств.</span><span class="sxs-lookup"><span data-stu-id="02346-155">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="02346-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="02346-156">Response</span></span>
<span data-ttu-id="02346-157">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="02346-157">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02346-158">Пример</span><span class="sxs-lookup"><span data-stu-id="02346-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="02346-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="02346-159">Request</span></span>
<span data-ttu-id="02346-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02346-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
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

### <a name="response"></a><span data-ttu-id="02346-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="02346-161">Response</span></span>
<span data-ttu-id="02346-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02346-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





