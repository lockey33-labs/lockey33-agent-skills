# Skill — Memory Persistence

## Purpose

Ce skill permet à Diego de sauvegarder et restaurer le contexte des sessions précédentes.

## Usage

### Sauvegarder la mémoire

```bash
# Copier la mémoire courante vers le skill
cp /root/.agent-memory/context.md /home/agent/lockey33-agent-skills/memory/context.md

# Commit et push
cd /home/agent/lockey33-agent-skills/
git add memory/context.md
git commit -m "docs: mise à jour mémoire $(date -u +%Y-%m-%d)"
git push origin main
```

### Restaurer la mémoire

```bash
cp /home/agent/lockey33-agent-skills/memory/context.md /root/.agent-memory/context.md
```

## Structure de la mémoire

Le fichier `context.md` contient:
- **Contexte de session** — Décisions importantes, état des projets
- **Configuration système** — Cron jobs, services, scripts persistants
- **Liens Notion** — URLs importantes pour la documentation
- **Prochains objectifs** — Actions à réaliser

## Dernière mise à jour

**Date** : 2026-03-07
**Session** : Auto-Research Loop & URL Shortener Decision
