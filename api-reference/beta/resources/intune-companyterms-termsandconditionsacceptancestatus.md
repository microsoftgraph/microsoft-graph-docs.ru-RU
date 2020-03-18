---
title: Тип ресурса termsAndConditionsAcceptanceStatus
description: Объект termsAndConditionsAcceptanceStatus представляет состояние принятия определенной политики условий для заданного пользователя. Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e40a20c65f490c67a0fc940f8b4bd7701863b450
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797271"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="b7c27-104">Тип ресурса termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="b7c27-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="b7c27-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7c27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7c27-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7c27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7c27-107">Объект termsAndConditionsAcceptanceStatus представляет состояние принятия определенной политики условий для заданного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b7c27-107">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="b7c27-108">Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.</span><span class="sxs-lookup"><span data-stu-id="b7c27-108">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>

## <a name="methods"></a><span data-ttu-id="b7c27-109">Методы</span><span class="sxs-lookup"><span data-stu-id="b7c27-109">Methods</span></span>
|<span data-ttu-id="b7c27-110">Метод</span><span class="sxs-lookup"><span data-stu-id="b7c27-110">Method</span></span>|<span data-ttu-id="b7c27-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b7c27-111">Return Type</span></span>|<span data-ttu-id="b7c27-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b7c27-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b7c27-113">Список termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="b7c27-113">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="b7c27-114">Коллекция [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span><span class="sxs-lookup"><span data-stu-id="b7c27-114">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="b7c27-115">Список свойств и связей объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b7c27-115">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="b7c27-116">Получение объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="b7c27-116">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|<span data-ttu-id="b7c27-117">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md);</span><span class="sxs-lookup"><span data-stu-id="b7c27-117">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span></span>|<span data-ttu-id="b7c27-118">Чтение свойств и связей объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b7c27-118">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="b7c27-119">Создание объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="b7c27-119">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|<span data-ttu-id="b7c27-120">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md);</span><span class="sxs-lookup"><span data-stu-id="b7c27-120">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span></span>|<span data-ttu-id="b7c27-121">Создание объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b7c27-121">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="b7c27-122">Удаление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="b7c27-122">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="b7c27-123">Нет</span><span class="sxs-lookup"><span data-stu-id="b7c27-123">None</span></span>|<span data-ttu-id="b7c27-124">Удаляет объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b7c27-124">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="b7c27-125">Обновление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="b7c27-125">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="b7c27-126">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="b7c27-126">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="b7c27-127">Обновление свойств объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b7c27-127">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b7c27-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7c27-128">Properties</span></span>
|<span data-ttu-id="b7c27-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7c27-129">Property</span></span>|<span data-ttu-id="b7c27-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b7c27-130">Type</span></span>|<span data-ttu-id="b7c27-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b7c27-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7c27-132">id</span><span class="sxs-lookup"><span data-stu-id="b7c27-132">id</span></span>|<span data-ttu-id="b7c27-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b7c27-133">String</span></span>|<span data-ttu-id="b7c27-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="b7c27-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="b7c27-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b7c27-135">userDisplayName</span></span>|<span data-ttu-id="b7c27-136">String</span><span class="sxs-lookup"><span data-stu-id="b7c27-136">String</span></span>|<span data-ttu-id="b7c27-137">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="b7c27-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="b7c27-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="b7c27-138">acceptedVersion</span></span>|<span data-ttu-id="b7c27-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b7c27-139">Int32</span></span>|<span data-ttu-id="b7c27-140">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="b7c27-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="b7c27-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7c27-141">acceptedDateTime</span></span>|<span data-ttu-id="b7c27-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7c27-142">DateTimeOffset</span></span>|<span data-ttu-id="b7c27-143">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="b7c27-143">DateTime when the terms were last accepted by the user.</span></span>|
|<span data-ttu-id="b7c27-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b7c27-144">userPrincipalName</span></span>|<span data-ttu-id="b7c27-145">String</span><span class="sxs-lookup"><span data-stu-id="b7c27-145">String</span></span>|<span data-ttu-id="b7c27-146">UserPrincipalName пользователя, который принял термин.</span><span class="sxs-lookup"><span data-stu-id="b7c27-146">The userPrincipalName of the User that accepted the term.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7c27-147">Связи</span><span class="sxs-lookup"><span data-stu-id="b7c27-147">Relationships</span></span>
|<span data-ttu-id="b7c27-148">Связь</span><span class="sxs-lookup"><span data-stu-id="b7c27-148">Relationship</span></span>|<span data-ttu-id="b7c27-149">Тип</span><span class="sxs-lookup"><span data-stu-id="b7c27-149">Type</span></span>|<span data-ttu-id="b7c27-150">Описание</span><span class="sxs-lookup"><span data-stu-id="b7c27-150">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7c27-151">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="b7c27-151">termsAndConditions</span></span>|[<span data-ttu-id="b7c27-152">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="b7c27-152">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="b7c27-153">Ссылка для перехода к назначенным условиям.</span><span class="sxs-lookup"><span data-stu-id="b7c27-153">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7c27-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7c27-154">JSON Representation</span></span>
<span data-ttu-id="b7c27-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7c27-155">Here is a JSON representation of the resource.</span></span>
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



