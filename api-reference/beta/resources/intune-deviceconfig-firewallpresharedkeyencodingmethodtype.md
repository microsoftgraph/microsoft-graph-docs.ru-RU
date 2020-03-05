---
title: тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе
description: Возможные значения для Фиреваллпрешаредкэйенкодингмесод
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0e2b5a3094ea0e5f351d67968254250156f98453
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526439"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="9a9ad-103">тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="9a9ad-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="9a9ad-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9a9ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a9ad-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a9ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a9ad-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a9ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a9ad-107">Возможные значения для Фиреваллпрешаредкэйенкодингмесод</span><span class="sxs-lookup"><span data-stu-id="9a9ad-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="9a9ad-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9a9ad-108">Members</span></span>
|<span data-ttu-id="9a9ad-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9a9ad-109">Member</span></span>|<span data-ttu-id="9a9ad-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9a9ad-110">Value</span></span>|<span data-ttu-id="9a9ad-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9a9ad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a9ad-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="9a9ad-112">deviceDefault</span></span>|<span data-ttu-id="9a9ad-113">нуль</span><span class="sxs-lookup"><span data-stu-id="9a9ad-113">0</span></span>|<span data-ttu-id="9a9ad-114">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="9a9ad-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="9a9ad-115">нет</span><span class="sxs-lookup"><span data-stu-id="9a9ad-115">none</span></span>|<span data-ttu-id="9a9ad-116">1 </span><span class="sxs-lookup"><span data-stu-id="9a9ad-116">1</span></span>|<span data-ttu-id="9a9ad-117">Общий ключ не кодируется.</span><span class="sxs-lookup"><span data-stu-id="9a9ad-117">Preshared key is not encoded.</span></span> <span data-ttu-id="9a9ad-118">Вместо этого он хранится в расширенном формате символов</span><span class="sxs-lookup"><span data-stu-id="9a9ad-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="9a9ad-119">utF8</span><span class="sxs-lookup"><span data-stu-id="9a9ad-119">utF8</span></span>|<span data-ttu-id="9a9ad-120">2 </span><span class="sxs-lookup"><span data-stu-id="9a9ad-120">2</span></span>|<span data-ttu-id="9a9ad-121">Кодирование общего ключа с помощью UTF – 8</span><span class="sxs-lookup"><span data-stu-id="9a9ad-121">Encode the preshared key using UTF-8</span></span>|



