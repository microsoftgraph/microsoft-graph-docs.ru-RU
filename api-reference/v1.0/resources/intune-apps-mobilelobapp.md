---
title: Тип ресурса mobileLobApp
description: Абстрактный базовый класс, содержащий свойства для всех мобильных бизнес-приложений.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1003d8e7e2ef0295f7635b478a0e5de32cf3414a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439654"
---
# <a name="mobilelobapp-resource-type"></a><span data-ttu-id="224b3-103">Тип ресурса mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="224b3-103">mobileLobApp resource type</span></span>

<span data-ttu-id="224b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="224b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="224b3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="224b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="224b3-106">Абстрактный базовый класс, содержащий свойства для всех мобильных бизнес-приложений.</span><span class="sxs-lookup"><span data-stu-id="224b3-106">An abstract base class containing properties for all mobile line of business apps.</span></span>


<span data-ttu-id="224b3-107">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-107">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="224b3-108">Методы</span><span class="sxs-lookup"><span data-stu-id="224b3-108">Methods</span></span>
|<span data-ttu-id="224b3-109">Метод</span><span class="sxs-lookup"><span data-stu-id="224b3-109">Method</span></span>|<span data-ttu-id="224b3-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="224b3-110">Return Type</span></span>|<span data-ttu-id="224b3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="224b3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="224b3-112">Перечисление mobileLobApps</span><span class="sxs-lookup"><span data-stu-id="224b3-112">List mobileLobApps</span></span>](../api/intune-apps-mobilelobapp-list.md)|<span data-ttu-id="224b3-113">Коллекция [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="224b3-113">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) collection</span></span>|<span data-ttu-id="224b3-114">Список свойств и связей объектов [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-114">List properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects.</span></span>|
|[<span data-ttu-id="224b3-115">Получение mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="224b3-115">Get mobileLobApp</span></span>](../api/intune-apps-mobilelobapp-get.md)|[<span data-ttu-id="224b3-116">mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="224b3-116">mobileLobApp</span></span>](../resources/intune-apps-mobilelobapp.md)|<span data-ttu-id="224b3-117">Считывание свойств и связей объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-117">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="224b3-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="224b3-118">Properties</span></span>
|<span data-ttu-id="224b3-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="224b3-119">Property</span></span>|<span data-ttu-id="224b3-120">Тип</span><span class="sxs-lookup"><span data-stu-id="224b3-120">Type</span></span>|<span data-ttu-id="224b3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="224b3-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="224b3-122">id</span><span class="sxs-lookup"><span data-stu-id="224b3-122">id</span></span>|<span data-ttu-id="224b3-123">Строка</span><span class="sxs-lookup"><span data-stu-id="224b3-123">String</span></span>|<span data-ttu-id="224b3-124">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="224b3-124">Key of the entity.</span></span> <span data-ttu-id="224b3-125">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-125">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="224b3-126">displayName</span><span class="sxs-lookup"><span data-stu-id="224b3-126">displayName</span></span>|<span data-ttu-id="224b3-127">Строка</span><span class="sxs-lookup"><span data-stu-id="224b3-127">String</span></span>|<span data-ttu-id="224b3-128">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="224b3-128">The admin provided or imported title of the app.</span></span> <span data-ttu-id="224b3-129">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-129">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="224b3-130">description</span><span class="sxs-lookup"><span data-stu-id="224b3-130">description</span></span>|<span data-ttu-id="224b3-131">Строка</span><span class="sxs-lookup"><span data-stu-id="224b3-131">String</span></span>|<span data-ttu-id="224b3-132">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="224b3-132">The description of the app.</span></span> <span data-ttu-id="224b3-133">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="224b3-134">publisher</span><span class="sxs-lookup"><span data-stu-id="224b3-134">publisher</span></span>|<span data-ttu-id="224b3-135">String</span><span class="sxs-lookup"><span data-stu-id="224b3-135">String</span></span>|<span data-ttu-id="224b3-136">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="224b3-136">The publisher of the app.</span></span> <span data-ttu-id="224b3-137">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="224b3-138">largeIcon</span><span class="sxs-lookup"><span data-stu-id="224b3-138">largeIcon</span></span>|[<span data-ttu-id="224b3-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="224b3-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="224b3-140">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="224b3-140">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="224b3-141">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="224b3-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="224b3-142">createdDateTime</span></span>|<span data-ttu-id="224b3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="224b3-143">DateTimeOffset</span></span>|<span data-ttu-id="224b3-144">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="224b3-144">The date and time the app was created.</span></span> <span data-ttu-id="224b3-145">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="224b3-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="224b3-146">lastModifiedDateTime</span></span>|<span data-ttu-id="224b3-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="224b3-147">DateTimeOffset</span></span>|<span data-ttu-id="224b3-148">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="224b3-148">The date and time the app was last modified.</span></span> <span data-ttu-id="224b3-149">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="224b3-150">isFeatured</span><span class="sxs-lookup"><span data-stu-id="224b3-150">isFeatured</span></span>|<span data-ttu-id="224b3-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="224b3-151">Boolean</span></span>|<span data-ttu-id="224b3-152">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-152">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="224b3-153">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="224b3-153">privacyInformationUrl</span></span>|<span data-ttu-id="224b3-154">String</span><span class="sxs-lookup"><span data-stu-id="224b3-154">String</span></span>|<span data-ttu-id="224b3-155">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="224b3-155">The privacy statement Url.</span></span> <span data-ttu-id="224b3-156">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="224b3-157">informationUrl</span><span class="sxs-lookup"><span data-stu-id="224b3-157">informationUrl</span></span>|<span data-ttu-id="224b3-158">String</span><span class="sxs-lookup"><span data-stu-id="224b3-158">String</span></span>|<span data-ttu-id="224b3-159">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="224b3-159">The more information Url.</span></span> <span data-ttu-id="224b3-160">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="224b3-161">owner</span><span class="sxs-lookup"><span data-stu-id="224b3-161">owner</span></span>|<span data-ttu-id="224b3-162">String</span><span class="sxs-lookup"><span data-stu-id="224b3-162">String</span></span>|<span data-ttu-id="224b3-163">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="224b3-163">The owner of the app.</span></span> <span data-ttu-id="224b3-164">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="224b3-165">developer</span><span class="sxs-lookup"><span data-stu-id="224b3-165">developer</span></span>|<span data-ttu-id="224b3-166">String</span><span class="sxs-lookup"><span data-stu-id="224b3-166">String</span></span>|<span data-ttu-id="224b3-167">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="224b3-167">The developer of the app.</span></span> <span data-ttu-id="224b3-168">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="224b3-169">notes</span><span class="sxs-lookup"><span data-stu-id="224b3-169">notes</span></span>|<span data-ttu-id="224b3-170">String</span><span class="sxs-lookup"><span data-stu-id="224b3-170">String</span></span>|<span data-ttu-id="224b3-171">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="224b3-171">Notes for the app.</span></span> <span data-ttu-id="224b3-172">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="224b3-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="224b3-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="224b3-173">publishingState</span></span>|[<span data-ttu-id="224b3-174">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="224b3-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="224b3-175">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="224b3-175">The publishing state for the app.</span></span> <span data-ttu-id="224b3-176">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="224b3-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="224b3-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="224b3-178">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="224b3-178">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="224b3-179">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="224b3-179">committedContentVersion</span></span>|<span data-ttu-id="224b3-180">String</span><span class="sxs-lookup"><span data-stu-id="224b3-180">String</span></span>|<span data-ttu-id="224b3-181">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="224b3-181">The internal committed content version.</span></span>|
|<span data-ttu-id="224b3-182">fileName</span><span class="sxs-lookup"><span data-stu-id="224b3-182">fileName</span></span>|<span data-ttu-id="224b3-183">String</span><span class="sxs-lookup"><span data-stu-id="224b3-183">String</span></span>|<span data-ttu-id="224b3-184">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="224b3-184">The name of the main Lob application file.</span></span>|
|<span data-ttu-id="224b3-185">size</span><span class="sxs-lookup"><span data-stu-id="224b3-185">size</span></span>|<span data-ttu-id="224b3-186">Int64</span><span class="sxs-lookup"><span data-stu-id="224b3-186">Int64</span></span>|<span data-ttu-id="224b3-187">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="224b3-187">The total size, including all uploaded files.</span></span>|

## <a name="relationships"></a><span data-ttu-id="224b3-188">Отношения</span><span class="sxs-lookup"><span data-stu-id="224b3-188">Relationships</span></span>
|<span data-ttu-id="224b3-189">Связь</span><span class="sxs-lookup"><span data-stu-id="224b3-189">Relationship</span></span>|<span data-ttu-id="224b3-190">Тип</span><span class="sxs-lookup"><span data-stu-id="224b3-190">Type</span></span>|<span data-ttu-id="224b3-191">Описание</span><span class="sxs-lookup"><span data-stu-id="224b3-191">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="224b3-192">categories</span><span class="sxs-lookup"><span data-stu-id="224b3-192">categories</span></span>|<span data-ttu-id="224b3-193">Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="224b3-193">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="224b3-194">Список категорий для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="224b3-194">The list of categories for this app.</span></span> <span data-ttu-id="224b3-195">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-195">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="224b3-196">assignments</span><span class="sxs-lookup"><span data-stu-id="224b3-196">assignments</span></span>|<span data-ttu-id="224b3-197">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="224b3-197">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="224b3-198">Список назначений группы для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="224b3-198">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="224b3-199">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="224b3-199">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="224b3-200">contentVersions</span><span class="sxs-lookup"><span data-stu-id="224b3-200">contentVersions</span></span>|<span data-ttu-id="224b3-201">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="224b3-201">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="224b3-202">Список версий содержимого для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="224b3-202">The list of content versions for this app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="224b3-203">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="224b3-203">JSON Representation</span></span>
<span data-ttu-id="224b3-204">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="224b3-204">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileLobApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024
}
```







