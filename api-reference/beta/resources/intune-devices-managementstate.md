---
title: тип переуправления managementState
description: Состояние управления устройством в Microsoft Intune.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f7ce0bedbc6376e6ae4205af71a968f9f976a48e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125822"
---
# <a name="managementstate-enum-type"></a>тип переуправления managementState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние управления устройством в Microsoft Intune.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|управляемый|0|Устройство находится под управлением|
|retirePending|1|На устройстве и в процессе отгрузки из управления возникает команда по отставку|
|retireFailed|2|На устройстве сбой команды по отставку|
|wipePending|3|Команда wipe происходит на устройстве и в процессе отгрузки из управления|
|wipeFailed|4 |Команда Wipe сбой на устройстве|
|нездоровый|5 |Устройство является нездоровым.|
|deletePending|6 |На устройстве возникает команда удаления |
|retireIssued|7 |Для устройства была выдана команда на отставку|
|wipeIssued|8 |Для устройства была выдана команда wipe|
|wipeCanceled|9 |Команда wipe для этого устройства отменена|
|retireCanceled|10 |Команда отмены для этого устройства отменена|
|обнаружено|11|Устройство обнаружено, но не полностью зарегистрировано.|



