---
title: Тип ресурса user
description: Представляет объект пользователя Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b5f9c0ab08db3c8b9f6e48138e31d091ab5dde9a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755551"
---
# <a name="user-resource-type"></a><span data-ttu-id="ca639-103">Тип ресурса user</span><span class="sxs-lookup"><span data-stu-id="ca639-103">user resource type</span></span>

<span data-ttu-id="ca639-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca639-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca639-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca639-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca639-106">Представляет объект пользователя Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ca639-106">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="ca639-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ca639-107">Methods</span></span>
|<span data-ttu-id="ca639-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ca639-108">Method</span></span>|<span data-ttu-id="ca639-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ca639-109">Return Type</span></span>|<span data-ttu-id="ca639-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ca639-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ca639-111">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="ca639-111">List users</span></span>](../api/intune-mam-user-list.md)|<span data-ttu-id="ca639-112">Коллекция объектов [user](../resources/intune-mam-user.md)</span><span class="sxs-lookup"><span data-stu-id="ca639-112">[user](../resources/intune-mam-user.md) collection</span></span>|<span data-ttu-id="ca639-113">Список свойств и связей объектов [user](../resources/intune-mam-user.md).</span><span class="sxs-lookup"><span data-stu-id="ca639-113">List properties and relationships of the [user](../resources/intune-mam-user.md) objects.</span></span>|
|[<span data-ttu-id="ca639-114">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="ca639-114">Get user</span></span>](../api/intune-mam-user-get.md)|[<span data-ttu-id="ca639-115">user</span><span class="sxs-lookup"><span data-stu-id="ca639-115">user</span></span>](../resources/intune-mam-user.md)|<span data-ttu-id="ca639-116">Чтение свойств и связей объекта [user](../resources/intune-mam-user.md).</span><span class="sxs-lookup"><span data-stu-id="ca639-116">Read properties and relationships of the [user](../resources/intune-mam-user.md) object.</span></span>|
|[<span data-ttu-id="ca639-117">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="ca639-117">Create user</span></span>](../api/intune-mam-user-create.md)|[<span data-ttu-id="ca639-118">user</span><span class="sxs-lookup"><span data-stu-id="ca639-118">user</span></span>](../resources/intune-mam-user.md)|<span data-ttu-id="ca639-119">Создание объекта [user](../resources/intune-mam-user.md).</span><span class="sxs-lookup"><span data-stu-id="ca639-119">Create a new [user](../resources/intune-mam-user.md) object.</span></span>|
|[<span data-ttu-id="ca639-120">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="ca639-120">Delete user</span></span>](../api/intune-mam-user-delete.md)|<span data-ttu-id="ca639-121">Нет</span><span class="sxs-lookup"><span data-stu-id="ca639-121">None</span></span>|<span data-ttu-id="ca639-122">Удаляет объект [user](../resources/intune-mam-user.md).</span><span class="sxs-lookup"><span data-stu-id="ca639-122">Deletes a [user](../resources/intune-mam-user.md).</span></span>|
|[<span data-ttu-id="ca639-123">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="ca639-123">Update user</span></span>](../api/intune-mam-user-update.md)|[<span data-ttu-id="ca639-124">user</span><span class="sxs-lookup"><span data-stu-id="ca639-124">user</span></span>](../resources/intune-mam-user.md)|<span data-ttu-id="ca639-125">Обновление свойств объекта [user](../resources/intune-mam-user.md).</span><span class="sxs-lookup"><span data-stu-id="ca639-125">Update the properties of a [user](../resources/intune-mam-user.md) object.</span></span>|
|[<span data-ttu-id="ca639-126">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="ca639-126">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-mam-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="ca639-127">Коллекция [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)</span><span class="sxs-lookup"><span data-stu-id="ca639-127">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="ca639-128">Получает состояние диагностической проверки определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca639-128">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="ca639-129">Функция getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="ca639-129">getManagedAppPolicies function</span></span>](../api/intune-mam-user-getmanagedapppolicies.md)|<span data-ttu-id="ca639-130">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ca639-130">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="ca639-131">Получает ограничения приложений для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca639-131">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="ca639-132">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="ca639-132">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-mam-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="ca639-133">Нет</span><span class="sxs-lookup"><span data-stu-id="ca639-133">None</span></span>|<span data-ttu-id="ca639-134">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="ca639-134">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="ca639-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca639-135">Properties</span></span>
|<span data-ttu-id="ca639-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca639-136">Property</span></span>|<span data-ttu-id="ca639-137">Тип</span><span class="sxs-lookup"><span data-stu-id="ca639-137">Type</span></span>|<span data-ttu-id="ca639-138">Описание</span><span class="sxs-lookup"><span data-stu-id="ca639-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca639-139">id</span><span class="sxs-lookup"><span data-stu-id="ca639-139">id</span></span>|<span data-ttu-id="ca639-140">String</span><span class="sxs-lookup"><span data-stu-id="ca639-140">String</span></span>|<span data-ttu-id="ca639-141">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca639-141">The user identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca639-142">Связи</span><span class="sxs-lookup"><span data-stu-id="ca639-142">Relationships</span></span>
|<span data-ttu-id="ca639-143">Связь</span><span class="sxs-lookup"><span data-stu-id="ca639-143">Relationship</span></span>|<span data-ttu-id="ca639-144">Тип</span><span class="sxs-lookup"><span data-stu-id="ca639-144">Type</span></span>|<span data-ttu-id="ca639-145">Описание</span><span class="sxs-lookup"><span data-stu-id="ca639-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca639-146">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="ca639-146">managedAppRegistrations</span></span>|<span data-ttu-id="ca639-147">Коллекция [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="ca639-147">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="ca639-148">Любое количество объектов регистрации управляемых приложений, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="ca639-148">Zero or more managed app registrations that belong to the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca639-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca639-149">JSON Representation</span></span>
<span data-ttu-id="ca639-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca639-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```




