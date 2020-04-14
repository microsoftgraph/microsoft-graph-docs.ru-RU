---
title: тип перечисления Граупполициоператионтипе
description: Тип операции с групповой политикой.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a14505e31f9e36a41237a578158d8ddcdbef909b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446936"
---
# <a name="grouppolicyoperationtype-enum-type"></a><span data-ttu-id="23374-103">тип перечисления Граупполициоператионтипе</span><span class="sxs-lookup"><span data-stu-id="23374-103">groupPolicyOperationType enum type</span></span>

<span data-ttu-id="23374-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23374-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23374-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23374-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23374-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23374-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23374-107">Тип операции с групповой политикой.</span><span class="sxs-lookup"><span data-stu-id="23374-107">Type of Group Policy operation.</span></span>

## <a name="members"></a><span data-ttu-id="23374-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="23374-108">Members</span></span>
|<span data-ttu-id="23374-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="23374-109">Member</span></span>|<span data-ttu-id="23374-110">Значение</span><span class="sxs-lookup"><span data-stu-id="23374-110">Value</span></span>|<span data-ttu-id="23374-111">Описание</span><span class="sxs-lookup"><span data-stu-id="23374-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23374-112">нет</span><span class="sxs-lookup"><span data-stu-id="23374-112">none</span></span>|<span data-ttu-id="23374-113">нуль</span><span class="sxs-lookup"><span data-stu-id="23374-113">0</span></span>|<span data-ttu-id="23374-114">Групповая политика: недопустимый тип операции.</span><span class="sxs-lookup"><span data-stu-id="23374-114">Group Policy invalid operation type.</span></span>|
|<span data-ttu-id="23374-115">загрузку</span><span class="sxs-lookup"><span data-stu-id="23374-115">upload</span></span>|<span data-ttu-id="23374-116">1,1</span><span class="sxs-lookup"><span data-stu-id="23374-116">1</span></span>|<span data-ttu-id="23374-117">Тип операции отправки групповой политики.</span><span class="sxs-lookup"><span data-stu-id="23374-117">Group Policy upload operation type.</span></span>|
|<span data-ttu-id="23374-118">уплоадневверсион</span><span class="sxs-lookup"><span data-stu-id="23374-118">uploadNewVersion</span></span>|<span data-ttu-id="23374-119">2</span><span class="sxs-lookup"><span data-stu-id="23374-119">2</span></span>|<span data-ttu-id="23374-120">Отправка типа операции новой версии групповой политики.</span><span class="sxs-lookup"><span data-stu-id="23374-120">Group Policy upload new version operation type.</span></span>|
|<span data-ttu-id="23374-121">аддлангуажефилес</span><span class="sxs-lookup"><span data-stu-id="23374-121">addLanguageFiles</span></span>|<span data-ttu-id="23374-122">4</span><span class="sxs-lookup"><span data-stu-id="23374-122">3</span></span>|<span data-ttu-id="23374-123">Тип операции "Добавление файлов нового языка" групповой политики (ADML).</span><span class="sxs-lookup"><span data-stu-id="23374-123">Group Policy add new language(ADML) files operation type.</span></span>|
|<span data-ttu-id="23374-124">ремовелангуажефилес</span><span class="sxs-lookup"><span data-stu-id="23374-124">removeLanguageFiles</span></span>|<span data-ttu-id="23374-125">4 </span><span class="sxs-lookup"><span data-stu-id="23374-125">4</span></span>|<span data-ttu-id="23374-126">Тип операции удаления файлов на языке групповой политики (ADML).</span><span class="sxs-lookup"><span data-stu-id="23374-126">Group Policy remove language(ADML) files operation type.</span></span>|
|<span data-ttu-id="23374-127">упдателангуажефилес</span><span class="sxs-lookup"><span data-stu-id="23374-127">updateLanguageFiles</span></span>|<span data-ttu-id="23374-128">5 </span><span class="sxs-lookup"><span data-stu-id="23374-128">5</span></span>|<span data-ttu-id="23374-129">Тип операции для файлов на языке обновлений групповой политики (ADML).</span><span class="sxs-lookup"><span data-stu-id="23374-129">Group Policy update language(ADML) files operation type.</span></span>|
|<span data-ttu-id="23374-130">удалить</span><span class="sxs-lookup"><span data-stu-id="23374-130">remove</span></span>|<span data-ttu-id="23374-131">6 </span><span class="sxs-lookup"><span data-stu-id="23374-131">6</span></span>|<span data-ttu-id="23374-132">Групповая политика удалить отправленный тип операции с файлами.</span><span class="sxs-lookup"><span data-stu-id="23374-132">Group Policy remove uploaded file operation type.</span></span>|



