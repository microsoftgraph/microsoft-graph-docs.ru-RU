---
author: JeremyKelley
description: Элементы данных, связанные с приглашением, группы ресурсов SharingInvitation в одну структуру.
ms.date: 09/10/2017
title: SharingInvitation
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: db2214132dcbecdfb8b8689bdb3d5547a13be2ab
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723279"
---
# <a name="sharinginvitation-resource-type"></a>Тип ресурса SharingInvitation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Элементы **данных, связанные с** приглашением, группы ресурсов SharingInvitation в одну структуру.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingInvitation"
}-->

```json
{
  "email": "string",
  "invitedBy": {"@odata.type": "microsoft.graph.identitySet" },
  "signInRequired": true
}

```

## <a name="properties"></a>Свойства

| Свойство       | Тип                          | Описание                                                                                                                   |
| :------------- | :---------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| email          | String                        | Электронный адрес получателя приглашения к совместному использованию. Только для чтения.                                            |
| invitedBy      | [identitySet](identityset.md) | Предоставляет сведения об отправителе приглашения, создавшего данное разрешение (если такие сведения доступны). Только для чтения. |
| signInRequired | Boolean                       | Значение `true` указывает, что получатель приглашения должен выполнить вход для доступа к предоставленному элементу. Только для чтения.                     |

## <a name="remarks"></a>Заметки

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
