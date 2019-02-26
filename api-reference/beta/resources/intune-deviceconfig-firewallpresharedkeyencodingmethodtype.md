---
title: тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе
description: Возможные значения для Фиреваллпрешаредкэйенкодингмесод
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e3a74122f0b0a9fe1a6dfab40593123ec8709c5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160818"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="b7d04-103">тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="b7d04-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="b7d04-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7d04-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7d04-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7d04-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7d04-106">Возможные значения для Фиреваллпрешаредкэйенкодингмесод</span><span class="sxs-lookup"><span data-stu-id="b7d04-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="b7d04-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b7d04-107">Members</span></span>
|<span data-ttu-id="b7d04-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b7d04-108">Member</span></span>|<span data-ttu-id="b7d04-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b7d04-109">Value</span></span>|<span data-ttu-id="b7d04-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b7d04-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7d04-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="b7d04-111">deviceDefault</span></span>|<span data-ttu-id="b7d04-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b7d04-112">0</span></span>|<span data-ttu-id="b7d04-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="b7d04-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="b7d04-114">Нет</span><span class="sxs-lookup"><span data-stu-id="b7d04-114">none</span></span>|<span data-ttu-id="b7d04-115">1,1</span><span class="sxs-lookup"><span data-stu-id="b7d04-115">1</span></span>|<span data-ttu-id="b7d04-116">Общий ключ не кодируется.</span><span class="sxs-lookup"><span data-stu-id="b7d04-116">Preshared key is not encoded.</span></span> <span data-ttu-id="b7d04-117">Вместо этого он хранится в расширенном формате символов</span><span class="sxs-lookup"><span data-stu-id="b7d04-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="b7d04-118">utF8</span><span class="sxs-lookup"><span data-stu-id="b7d04-118">utF8</span></span>|<span data-ttu-id="b7d04-119">2</span><span class="sxs-lookup"><span data-stu-id="b7d04-119">2</span></span>|<span data-ttu-id="b7d04-120">Кодирование общего ключа с помощью UTF – 8</span><span class="sxs-lookup"><span data-stu-id="b7d04-120">Encode the preshared key using UTF-8</span></span>|




