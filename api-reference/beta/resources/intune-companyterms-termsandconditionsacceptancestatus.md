---
title: Тип ресурса termsAndConditionsAcceptanceStatus
description: Объект termsAndConditionsAcceptanceStatus представляет состояние принятия определенной политики условий для заданного пользователя. Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 232f7277479d1e6fa558deb0b365ca90d9522675
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42487783"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="30cb4-104">Тип ресурса termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="30cb4-104">termsAndConditionsAcceptanceStatus resource type</span></span>

<span data-ttu-id="30cb4-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="30cb4-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30cb4-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30cb4-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30cb4-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30cb4-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30cb4-108">Объект termsAndConditionsAcceptanceStatus представляет состояние принятия определенной политики условий для заданного пользователя.</span><span class="sxs-lookup"><span data-stu-id="30cb4-108">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="30cb4-109">Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.</span><span class="sxs-lookup"><span data-stu-id="30cb4-109">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>

## <a name="methods"></a><span data-ttu-id="30cb4-110">Методы</span><span class="sxs-lookup"><span data-stu-id="30cb4-110">Methods</span></span>
|<span data-ttu-id="30cb4-111">Метод</span><span class="sxs-lookup"><span data-stu-id="30cb4-111">Method</span></span>|<span data-ttu-id="30cb4-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="30cb4-112">Return Type</span></span>|<span data-ttu-id="30cb4-113">Описание</span><span class="sxs-lookup"><span data-stu-id="30cb4-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="30cb4-114">Список termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="30cb4-114">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="30cb4-115">Коллекция [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span><span class="sxs-lookup"><span data-stu-id="30cb4-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="30cb4-116">Список свойств и связей объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="30cb4-116">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="30cb4-117">Получение объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="30cb4-117">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|<span data-ttu-id="30cb4-118">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md);</span><span class="sxs-lookup"><span data-stu-id="30cb4-118">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span></span>|<span data-ttu-id="30cb4-119">Чтение свойств и связей объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="30cb4-119">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="30cb4-120">Создание объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="30cb4-120">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|<span data-ttu-id="30cb4-121">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md);</span><span class="sxs-lookup"><span data-stu-id="30cb4-121">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span></span>|<span data-ttu-id="30cb4-122">Создание объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="30cb4-122">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="30cb4-123">Удаление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="30cb4-123">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="30cb4-124">Нет</span><span class="sxs-lookup"><span data-stu-id="30cb4-124">None</span></span>|<span data-ttu-id="30cb4-125">Удаляет объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="30cb4-125">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="30cb4-126">Обновление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="30cb4-126">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="30cb4-127">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="30cb4-127">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="30cb4-128">Обновление свойств объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="30cb4-128">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="30cb4-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="30cb4-129">Properties</span></span>
|<span data-ttu-id="30cb4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="30cb4-130">Property</span></span>|<span data-ttu-id="30cb4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="30cb4-131">Type</span></span>|<span data-ttu-id="30cb4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="30cb4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30cb4-133">id</span><span class="sxs-lookup"><span data-stu-id="30cb4-133">id</span></span>|<span data-ttu-id="30cb4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="30cb4-134">String</span></span>|<span data-ttu-id="30cb4-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="30cb4-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="30cb4-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="30cb4-136">userDisplayName</span></span>|<span data-ttu-id="30cb4-137">String</span><span class="sxs-lookup"><span data-stu-id="30cb4-137">String</span></span>|<span data-ttu-id="30cb4-138">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="30cb4-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="30cb4-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="30cb4-139">acceptedVersion</span></span>|<span data-ttu-id="30cb4-140">Int32</span><span class="sxs-lookup"><span data-stu-id="30cb4-140">Int32</span></span>|<span data-ttu-id="30cb4-141">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="30cb4-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="30cb4-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="30cb4-142">acceptedDateTime</span></span>|<span data-ttu-id="30cb4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30cb4-143">DateTimeOffset</span></span>|<span data-ttu-id="30cb4-144">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="30cb4-144">DateTime when the terms were last accepted by the user.</span></span>|
|<span data-ttu-id="30cb4-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="30cb4-145">userPrincipalName</span></span>|<span data-ttu-id="30cb4-146">String</span><span class="sxs-lookup"><span data-stu-id="30cb4-146">String</span></span>|<span data-ttu-id="30cb4-147">UserPrincipalName пользователя, который принял термин.</span><span class="sxs-lookup"><span data-stu-id="30cb4-147">The userPrincipalName of the User that accepted the term.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30cb4-148">Связи</span><span class="sxs-lookup"><span data-stu-id="30cb4-148">Relationships</span></span>
|<span data-ttu-id="30cb4-149">Связь</span><span class="sxs-lookup"><span data-stu-id="30cb4-149">Relationship</span></span>|<span data-ttu-id="30cb4-150">Тип</span><span class="sxs-lookup"><span data-stu-id="30cb4-150">Type</span></span>|<span data-ttu-id="30cb4-151">Описание</span><span class="sxs-lookup"><span data-stu-id="30cb4-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30cb4-152">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="30cb4-152">termsAndConditions</span></span>|[<span data-ttu-id="30cb4-153">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="30cb4-153">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="30cb4-154">Ссылка для перехода к назначенным условиям.</span><span class="sxs-lookup"><span data-stu-id="30cb4-154">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30cb4-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30cb4-155">JSON Representation</span></span>
<span data-ttu-id="30cb4-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30cb4-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



