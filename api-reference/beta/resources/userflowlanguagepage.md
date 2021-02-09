---
title: Тип ресурса userFlowLanguagePage
description: Используемые страницы языка пользовательского потока определяют, какие строки пользователи будут показывать во время пользовательского пути, настроенного с помощью пользовательских потоков.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 25fb1c94db9443ed67a0555d09f3859e666bed19
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155470"
---
# <a name="userflowlanguagepage-resource-type"></a><span data-ttu-id="a8103-103">Тип ресурса userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="a8103-103">userFlowLanguagePage resource type</span></span>

<span data-ttu-id="a8103-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8103-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a8103-105">Используемые страницы языка пользовательского потока определяют, какие строки пользователи будут показывать во время пользовательского пути, настроенного с помощью пользовательских потоков.</span><span class="sxs-lookup"><span data-stu-id="a8103-105">User flow language pages are used determine the strings users will be shown during the user journey you have configured using user flows.</span></span> <span data-ttu-id="a8103-106">Эти языковые страницы включают как переводы языка по умолчанию, предоставляемые корпорацией Майкрософт, так и настраиваемые страницы, которые можно создать для настройки перевода языков.</span><span class="sxs-lookup"><span data-stu-id="a8103-106">These language pages include both the default language translations provided by Microsoft, or custom pages that can be created to customize the language translations.</span></span>

## <a name="methods"></a><span data-ttu-id="a8103-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a8103-107">Methods</span></span>

|<span data-ttu-id="a8103-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a8103-108">Method</span></span>|<span data-ttu-id="a8103-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="a8103-109">Return type</span></span>|<span data-ttu-id="a8103-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a8103-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a8103-111">Get userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="a8103-111">Get userFlowLanguagePage</span></span>](../api/userflowlanguagepage-get.md)|[<span data-ttu-id="a8103-112">userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="a8103-112">userFlowLanguagePage</span></span>](../resources/userflowlanguagepage.md)|<span data-ttu-id="a8103-113">Извлечение значений объекта [userFlowLanguagePage](../resources/userflowlanguagepage.md) по умолчанию или пользовательского объекта.</span><span class="sxs-lookup"><span data-stu-id="a8103-113">Retrieve the values of a default or custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|
|[<span data-ttu-id="a8103-114">Обновление userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="a8103-114">Update userFlowLanguagePage</span></span>](../api/userflowlanguagepage-put.md)|[<span data-ttu-id="a8103-115">userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="a8103-115">userFlowLanguagePage</span></span>](../resources/userflowlanguagepage.md)|<span data-ttu-id="a8103-116">Обновление значений в настраиваемом [объекте userFlowLanguagePage.](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="a8103-116">Update the values in a custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|
|[<span data-ttu-id="a8103-117">Удаление userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="a8103-117">Delete userFlowLanguagePage</span></span>](../api/userflowlanguagepage-delete.md)|<span data-ttu-id="a8103-118">Нет</span><span class="sxs-lookup"><span data-stu-id="a8103-118">None</span></span>|<span data-ttu-id="a8103-119">Удаляет значения из пользовательского [объекта userFlowLanguagePage.](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="a8103-119">Deletes the values from a custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a8103-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8103-120">Properties</span></span>

|<span data-ttu-id="a8103-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8103-121">Property</span></span>|<span data-ttu-id="a8103-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a8103-122">Type</span></span>|<span data-ttu-id="a8103-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a8103-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8103-124">id</span><span class="sxs-lookup"><span data-stu-id="a8103-124">id</span></span>|<span data-ttu-id="a8103-125">String</span><span class="sxs-lookup"><span data-stu-id="a8103-125">String</span></span>|<span data-ttu-id="a8103-126">Идентификатор страницы userFlowLanguage.</span><span class="sxs-lookup"><span data-stu-id="a8103-126">The identifier of the userFlowLanguage page.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8103-127">Связи</span><span class="sxs-lookup"><span data-stu-id="a8103-127">Relationships</span></span>

<span data-ttu-id="a8103-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a8103-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8103-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a8103-129">JSON representation</span></span>

<span data-ttu-id="a8103-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8103-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguagePage",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguagePage",
  "id": "String (identifier)"
}
```
