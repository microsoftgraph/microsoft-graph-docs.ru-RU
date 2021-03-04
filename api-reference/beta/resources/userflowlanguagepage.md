---
title: тип ресурса userFlowLanguagePage
description: Используются языковые страницы потока пользователей, которые определяют, какие строки будут показаны пользователям во время пользовательского путешествия, настроенного с помощью пользовательских потоков.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c76d746aabab06fcc68ffcead238aaf2cc6ddb41
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442717"
---
# <a name="userflowlanguagepage-resource-type"></a><span data-ttu-id="0af67-103">тип ресурса userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="0af67-103">userFlowLanguagePage resource type</span></span>

<span data-ttu-id="0af67-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0af67-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0af67-105">Используются языковые страницы потока пользователей, которые определяют, какие строки будут показаны пользователям во время пользовательского путешествия, настроенного с помощью пользовательских потоков.</span><span class="sxs-lookup"><span data-stu-id="0af67-105">User flow language pages are used determine the strings users will be shown during the user journey you have configured using user flows.</span></span> <span data-ttu-id="0af67-106">Эти языковые страницы включают как языковые переводы по умолчанию, предоставляемые Корпорацией Майкрософт, так и настраиваемые страницы, которые можно создать для настройки языковых переводов.</span><span class="sxs-lookup"><span data-stu-id="0af67-106">These language pages include both the default language translations provided by Microsoft, or custom pages that can be created to customize the language translations.</span></span>

## <a name="methods"></a><span data-ttu-id="0af67-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0af67-107">Methods</span></span>

|<span data-ttu-id="0af67-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0af67-108">Method</span></span>|<span data-ttu-id="0af67-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="0af67-109">Return type</span></span>|<span data-ttu-id="0af67-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0af67-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0af67-111">Get userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="0af67-111">Get userFlowLanguagePage</span></span>](../api/userflowlanguagepage-get.md)|[<span data-ttu-id="0af67-112">userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="0af67-112">userFlowLanguagePage</span></span>](../resources/userflowlanguagepage.md)|<span data-ttu-id="0af67-113">Извлечение значений объекта по умолчанию или [пользовательского пользователяFlowLanguagePage.](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="0af67-113">Retrieve the values of a default or custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|
|[<span data-ttu-id="0af67-114">Обновление userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="0af67-114">Update userFlowLanguagePage</span></span>](../api/userflowlanguagepage-put.md)|[<span data-ttu-id="0af67-115">userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="0af67-115">userFlowLanguagePage</span></span>](../resources/userflowlanguagepage.md)|<span data-ttu-id="0af67-116">Обновление значений в настраиваемом [объекте userFlowLanguagePage.](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="0af67-116">Update the values in a custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|
|[<span data-ttu-id="0af67-117">Удаление userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="0af67-117">Delete userFlowLanguagePage</span></span>](../api/userflowlanguagepage-delete.md)|<span data-ttu-id="0af67-118">Нет</span><span class="sxs-lookup"><span data-stu-id="0af67-118">None</span></span>|<span data-ttu-id="0af67-119">Удаляет значения из пользовательского [объекта userFlowLanguagePage.](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="0af67-119">Deletes the values from a custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0af67-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="0af67-120">Properties</span></span>

|<span data-ttu-id="0af67-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="0af67-121">Property</span></span>|<span data-ttu-id="0af67-122">Тип</span><span class="sxs-lookup"><span data-stu-id="0af67-122">Type</span></span>|<span data-ttu-id="0af67-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0af67-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0af67-124">id</span><span class="sxs-lookup"><span data-stu-id="0af67-124">id</span></span>|<span data-ttu-id="0af67-125">String</span><span class="sxs-lookup"><span data-stu-id="0af67-125">String</span></span>|<span data-ttu-id="0af67-126">Идентификатор страницы userFlowLanguage.</span><span class="sxs-lookup"><span data-stu-id="0af67-126">The identifier of the userFlowLanguage page.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0af67-127">Связи</span><span class="sxs-lookup"><span data-stu-id="0af67-127">Relationships</span></span>

<span data-ttu-id="0af67-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0af67-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0af67-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0af67-129">JSON representation</span></span>

<span data-ttu-id="0af67-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0af67-130">The following is a JSON representation of the resource.</span></span>
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
