---
title: тип переименовки remoteAssistanceOnboardingStatus
description: Текущее состояние соединиттеля TeamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d63300e02f1442a38bbcda7f8e211e9356b8e57
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755681"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>тип переименовки remoteAssistanceOnboardingStatus

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Текущее состояние соединиттеля TeamViewer

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notOnboarded|0|Состояние, сообщаемое при отсутствие активного соединитетеля TeamViewer, настроенного или активного|
|onboarding|1|Состояние, сообщалось, когда система инициировала подключение TeamViewer, но служба еще не завершила подтверждение соединитетеля|
|onboarded|2|Состояние, о чем сообщалось, когда система успешно обменивалась сведениями о учетных записях с TeamViewer и теперь может инициировать сеансы удаленной помощи с клиентами|




